<script lang="ts">
    
    interface Props {
        /**
     * Tiktokのプロフィールページへのリンク
     */
        url: string;
    }

    let { url }: Props = $props();
</script>

<div class="tiktok-logo">
    <a href={url} target="_blank">
        <img class="tiktok-button" src="icons/TikTok_Icon_Black_Circle.png" alt="TikTok Channel" />
    </a>
</div>

<style>
    .tiktok-button {
        width: 24px;
        height: 24px;
    }

    .tiktok-logo {
        padding: 0 15px;
    }
</style>