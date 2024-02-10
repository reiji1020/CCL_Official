<script>
    import { Header } from 'cclkit4svelte';
    import { Footer } from "cclkit4svelte";
    import SubTitle from "$lib/Subtitle.svelte";
    import ActivityLog from "$lib/ActivityLog.svelte";
    import Member from "$lib/Member.svelte";
</script>

<div class="ccl-header">
    <!--    HEADER      -->
    <a href="/">
        <Header bgColor="--strawberry-pink" height="--hd-nomal"/>
    </a>
</div>
<main>
    <!--    MainCard-->
    <SubTitle />
    <!--    ActivityLog-->
    <ActivityLog />
    <!--    Member-->
    <Member />
</main>
<div class="ccl-footer">
    <!--    FOOTER      -->
    <Footer bgColor="--strawberry-pink" />
</div>

<style lang="scss">
  .ccl-header{
    position: sticky;
    bottom: 100vh;
  }

  .ccl-footer{
    position: sticky;
    top: 100vh;
  }
</style>

