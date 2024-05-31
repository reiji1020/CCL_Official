<script>
    import { Table, Card, Footer, Header, CCLVividColor, HeaderHeight } from 'cclkit4svelte';
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
        <Header bgColor={CCLVividColor.STRAWBERRY_PINK} height={HeaderHeight.NOMAL}/>
    </a>
</div>
<main>
    <!--    MainCard-->
    <SubTitle/>
    <div class="activity-card-wrapper">
        <div class="card-padding">
            <a href="https://reiji1020.hatenablog.com/entry/2024/05/27/172504" target="_blank">
                <Card borderColor={CCLVividColor.PINEAPPLE_YELLOW} src="./Blog.png"
                      altText="汎用サムネイル画像" title="技術書典16オフラインイベント参加レポ"
                      cardText="技術書典16のオフラインイベントへサークル参加した際の振り返り記事を書きました。"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://gyaopan.booth.pm/items/5648807" target="_blank">
                <Card borderColor={CCLVividColor.STRAWBERRY_PINK} src="./Svelte.png"
                      altText="新刊「Svelte HTML CSS 三色丼」の書影" title="技術書典16の新刊を販売しています！"
                      cardText="技術書典16の新刊「Svelte HTML CSS 三色丼」販売中です。技術書典オンラインマーケット・BOOTHでお求めいだたけます!"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://github.com/reiji1020/ccl-component-kit4svelte" target="_blank">
                <Card borderColor={CCLVividColor.SODA_BLUE} src="./Programming.png"
                      altText="ProgrammingImage" title="Svelte製UIライブラリ開発中！"
                      cardText="完全Svelte製のUIコンポーネントライブラリ「cclkit4svelte」開発中です！"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://gyaopan.booth.pm/items/5793338" target="_blank">
                <Card borderColor={CCLVividColor.STRAWBERRY_PINK} src="./Writing.png"
                      altText="WritingImage" title="商業本のお知らせ"
                      cardText="CCLの技術同人誌を元に発行している商業誌のお知らせを掲載しています。"/>
            </a>
        </div>
    </div>
    <ActivityLog/>
    <div style="display: flex; justify-content: center; align-items: center">
        <Table tableColor={CCLVividColor.PINEAPPLE_YELLOW} dataHeader={updateTitle} tableData={updateData} />
    </div>
    <!--    Member-->
    <Member/>
    <Members/>
</main>
<div class="ccl-footer">
    <!--    FOOTER      -->
    <NavBar />
    <Footer bgColor={CCLVividColor.STRAWBERRY_PINK}/>
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

