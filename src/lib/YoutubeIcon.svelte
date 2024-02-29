<script lang="ts">
    /**
     * Xのプロフィールページへのリンク
     */
    export let url : string;
</script>

<div class="youtube-logo">
    <a href={url} target="_blank">
        <img src="icons/youtube_social_icon_white.png" alt="Youtube Channel" />
    </a>
</div>

<style>
    .youtube-logo {
        padding: 5px 0;
    }
</style>