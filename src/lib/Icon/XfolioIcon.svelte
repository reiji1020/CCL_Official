<script lang="ts">
    
    interface Props {
        /**
     * Xfolioのポートフォリオへのリンク
     */
        url: string;
    }

    let { url }: Props = $props();
</script>

<div class="xfolio-logo">
    <a href={url} target="_blank">
        <img class="xfolio-button" src="icons/Xfolio.jpg" alt="Xfolio logo" />
    </a>
</div>

<style>
    .xfolio-button {
        width: 58px;
        height: 24px;
    }

    .xfolio-logo {
        padding: 0 15px;
    }
</style>