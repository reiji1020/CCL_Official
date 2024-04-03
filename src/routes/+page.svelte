<script>
    import { Table, Card, Footer, Header} from 'cclkit4svelte';
    import SubTitle from "$lib/logo/Subtitle.svelte";
    import ActivityLog from "$lib/logo/ActivityLog.svelte";
    import Member from "$lib/logo/Member.svelte";
    import Members from "$lib/component/Members.svelte";
    import NavBar from "$lib/component/NavBar.svelte";

    import {updateTitle} from "$lib/assets/updateTableHeader.ts";
    import {updateData} from "$lib/assets/updateData.ts";
</script>

<div class="ccl-header">
    <!--    HEADER      -->
    <a href="/">
        <Header bgColor="--strawberry-pink" height="--hd-nomal"/>
    </a>
</div>
<main>
    <!--    MainCard-->
    <SubTitle/>
    <div class="activity-card-wrapper">
        <div class="card-padding">
            <a href="https://github.com/reiji1020/ccl-component-kit4svelte" target="_blank">
                <Card borderColor="--soda-blue" src="./thumbnail.png"
                      altText="Svelteコンポーネントライブラリ" title="UIライブラリ開発中！"
                      cardText="完全Svelte製のUIコンポーネントライブラリ「cclkit4svelte」開発中です！"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://reiji1020.hatenablog.com/entry/2024/03/15/210000" target="_blank">
                <Card borderColor="--pineapple-yellow" src="./thumbnail.png"
                      altText="CANDYCHUPSLab." title="技術書典16のオン・オフ参加決定！"
                      cardText="技術書典16のスペースを無事にいただくことができました！新刊情報は随時公開します。"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://nextpublishing.jp/book/13898.html" target="_blank">
                <Card borderColor="--strawberry-pink" src="./20240201.jpg"
                      altText="実践Reactコンポーネントライブラリ開発" title="新刊が発売されました！"
                      cardText="インプレスR&D様よりReactコンポーネントライブラリの本を出させていただきました。"/>
            </a>
        </div>
    </div>
    <ActivityLog/>
    <div style="display: flex; justify-content: center; align-items: center">
        <Table tableColor="--pineapple-yellow" dataHeader={updateTitle} tableData={updateData} />
    </div>
    <!--    Member-->
    <Member/>
    <Members/>
</main>
<div class="ccl-footer">
    <!--    FOOTER      -->
    <NavBar />
    <Footer bgColor="--strawberry-pink"/>
</div>

<style lang="scss">
  .ccl-header {
    position: sticky;
    bottom: 100vh;
  }

  .activity-card-wrapper {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }

  .card-padding {
    padding: 10px 0;
  }

  .ccl-footer {
    position: sticky;
    top: 100vh;
  }
</style>

