<script>
    import { Header } from 'cclkit4svelte';
    import { Footer } from "cclkit4svelte";
</script>

<div class="ccl-header">
    <a href="/">
        <Header bgColor="--strawberry-pink" height="--hd-nomal"/>
    </a>
</div>
<main>
    hogehoge
</main>
<div class="ccl-footer">
    <Footer class="ccl-footer" bgColor="--strawberry-pink" />
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

