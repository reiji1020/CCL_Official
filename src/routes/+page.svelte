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
        <Header bgColor={CCLVividColor.STRAWBERRY_PINK} height={HeaderHeight.NORMAL}/>
    </a>
</div>
<main>
    <!--    MainCard-->
    <SubTitle/>
    <div class="activity-card-wrapper">
        <div class="card-padding">
            <a href="https://cclshop.base.shop/items/98936642" target="_blank">
                <Card borderColor={CCLVividColor.PINEAPPLE_YELLOW} src="./bookmarks.jpeg"
                      altText="bookmarks image" title="新作ハンドメイド雑貨を販売しました"
                      cardText="おほしさまのビーズを使ったブックマーカーを作りました。各ショップで販売中です"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://bsky.app/profile/candychupslab.bsky.social/post/3lh64wzcwc22m" target="_blank">
                <Card borderColor={CCLVividColor.MELON_GREEN} src="./Writing.png"
                      altText="writing" title="技術書典18に参加申し込みをしました"
                      cardText="技術書典18へ申し込みました。今回もオフライン・オンライン両方に申し込んでいます。"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://nextpublishing.jp/book/17921.html" target="_blank">
                <Card borderColor={CCLVividColor.MELON_GREEN} src="./figma_svelte.jpg"
                      altText="FigmaSvelteCover" title="新刊(商業)のお知らせ"
                      cardText="インプレスNextPublishingさまより「FigmaとSvelteKitで学ぶやさしいWeb開発」を出版させていただきました！"/>
            </a>
        </div>
        <div class="card-padding">
            <a href="https://github.com/reiji1020/ccl-component-kit4svelte" target="_blank">
                <Card borderColor={CCLVividColor.GRAPE_PURPLE} src="./Programming.png"
                      altText="ProgrammingImage" title="Svelte製UIライブラリ開発中！"
                      cardText="完全Svelte製のUIコンポーネントライブラリ「cclkit4svelte」開発中です！"/>
            </a>
        </div>
<!--        <div class="card-padding">-->
<!--            <a href="https://gyaopan.booth.pm/items/5793338" target="_blank">-->
<!--                <Card borderColor={CCLVividColor.MELON_GREEN} src="./Writing.png"-->
<!--                      altText="WritingImage" title="商業本のお知らせ"-->
<!--                      cardText="CCLの技術同人誌を元に発行している商業誌のお知らせを掲載しています。"/>-->
<!--            </a>-->
<!--        </div>-->
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

