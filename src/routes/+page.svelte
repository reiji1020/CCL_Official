<script>
    import { Header, Footer, Card } from 'cclkit4svelte';
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
    <div class="activityCardWrapper">
        <Card borderColor="--pineapple-yellow" bgColor="--lemon-yellow" src="./thumbnail.png" altText="CANDYCHUPSLab." title="技術書典16にサークル参加を申し込みました！" cardText="2024年春に開催される技術書典16へサークル出典を申し込みました。Svelte関連の本が出ます。" />
        <Card borderColor="--strawberry-pink" bgColor="--peach-pink" src="./20240201.jpg" altText="実践Reactコンポーネントライブラリ開発" title="新刊が発売されました！" cardText="インプレスR&D様よりReactコンポーネントライブラリの本を出させていただきました。" />
        <Card borderColor="--strawberry-pink" bgColor="--peach-pink" src="./20221021.jpg" altText="実践入門ビジュアルプログラミング言語" title="vvvv&vvvv gamma本発売中！" cardText="各ネット書店でビジュアルプログラミング言語vvvvとvvvv gammaの本を発売中です。" />
    </div>
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

  .activityCardWrapper {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .ccl-footer{
    position: sticky;
    top: 100vh;
  }
</style>

