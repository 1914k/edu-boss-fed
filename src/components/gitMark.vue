<template>
  <ul>
    <li>添加远程仓库地址，并取别名为 origin: git remote add origin url地址</li>
    <li>查看远程仓库地址: git remote -v</li>
    <li>重命名仓库别名:  git remote rename origin newname</li>
    <li>推送代码到 origin 仓库的 master 分支上，下次推送时还是要带上 仓库名和分支名: git push origin master</li>
    <li>推送代码到 origin 仓库的 master 分支上，并后续默认推送到这里，直接 git push 就行: git push -u origin master</li>
  </ul>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
