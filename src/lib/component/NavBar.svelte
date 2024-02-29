<script lang="ts">
    import XIcon from "$lib/Icon/XIcon.svelte";
    import MisskeyIcon from "$lib/Icon/MisskeyIcon.svelte";
    import YoutubeIcon from "$lib/Icon/YoutubeIcon.svelte";
    import TiktokIcon from "$lib/Icon/TiktokIcon.svelte";
    import InstagramIcon from "$lib/Icon/InstagramIcon.svelte";
    import BoothIcon from "$lib/Icon/BoothIcon.svelte";
    import BaseIcon from "$lib/Icon/BaseIcon.svelte";
</script>

<div class="navbar-wrapper">
    <span class="title">SNS</span>
    <br />
    <div class="icon-wrapper">
        <XIcon url="https://twitter.com/candychupslab"/>
        <MisskeyIcon url="https://misskey.io/"/>
        <YoutubeIcon url="https://www.youtube.com/channel/UCI39kr4G1HU80T4fZZ8i9tw"/>
        <TiktokIcon url="https://www.tiktok.com/@candychupslab?lang=ja-JP" />
        <InstagramIcon url="https://www.instagram.com/candychupslab/"/>
    </div>
    <span class="title">SHOP</span>
    <br />
    <div class="icon-wrapper">
        <BaseIcon url="https://cclshop.base.shop/"/>
        <BoothIcon url="https://gyaopan.booth.pm/"/>
    </div>
</div>

<style>
    .navbar-wrapper {
        width: 100%;
        height: 256px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background: var(--strawberry-pink);
    }

    .title {
        font-size: 24px;
        color: #ffffff;
    }

    .icon-wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>