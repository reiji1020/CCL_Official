<script lang="ts">
    
    interface Props {
        /**
     * Youtubeのチャンネルページへのリンク
     */
        url: string;
    }

    let { url }: Props = $props();
</script>

<div class="youtube-logo">
    <a href={url} target="_blank">
        <img class="youtube-button" src="icons/youtube_social_icon_white.png" alt="Youtube Channel" />
    </a>
</div>

<style>
    .youtube-button {
        width: 32px;
        height: 23px;
    }

    .youtube-logo {
        padding: 0 15px;
    }
</style>