<script lang="ts">
    
    interface Props {
        /**
     * BASEのショップページへのリンク
     */
        url: string;
    }

    let { url }: Props = $props();
</script>

<div class="base-logo">
    <a href={url} target="_blank">
        <img class="base-button" src="icons/base_logo_horizontal_white.png" alt="BASE SHOP" />
    </a>
</div>

<style>
    .base-button {
        width: 60px;
        height: 24px;
    }

    .base-logo {
        padding: 0 15px;
    }
</style>