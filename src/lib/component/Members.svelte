<script lang="ts">
import { Thumbnail } from 'cclkit4svelte';
import XIcon from "$lib/Icon/XIcon.svelte";
import MisskeyIcon from "$lib/Icon/MisskeyIcon.svelte";
import YoutubeIcon from "$lib/Icon/YoutubeIcon.svelte";
import TwitchIcon from "$lib/Icon/TwitchIcon.svelte";
    </script>

<div class="members-wrapper">
    <div class="member-item">
        <Thumbnail borderColor="--soda-blue" altText="reiji1020" imageSize="256px" src="reiji1020.jpg" />
    </div>
    <div class="member-item">
        <span class="name">Saya Katafuchi (片渕 小夜)</span>
        <br />
        <span class="profile">Web Engineer & Designer</span>
        <br />
        <span class="profile">Tech Book Writer</span>
        <br />
        <span class="profile">Multi Creator</span>
        <br />
        <div class="sns-wrapper">
            <XIcon url="https://twitter.com/reiji1020"/>
            <MisskeyIcon url="https://misskey.io/@reiji1020" />
            <YoutubeIcon url="https://www.youtube.com/channel/UC5wBcqkoK3SGSrF4VRojcbQ" />
            <TwitchIcon url="https://www.twitch.tv/reiji1020" />
        </div>
    </div>
</div>

<style>
    .members-wrapper {
        width: 100%;
        height: 550px;
        display: flex;
        align-items: center;
        justify-content: center;
        background: var(--sugar-blue);
        flex-wrap: wrap;
    }

    .member-item {
        padding: 0 50px;
    }

    .name {
        font-size: 24px;
        color: var(--wrap-grey);
    }

    .profile {
        font-size: 18px;
        color: var(--wrap-grey);
    }

    .sns-wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>