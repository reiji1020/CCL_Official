<script lang="ts">
    
    interface Props {
        /**
     * Teitchのチャンネルページへのリンク
     */
        url: string;
    }

    let { url }: Props = $props();
</script>

<div class="twitch-logo">
    <a href={url} target="_blank">
        <svg id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
             viewBox="0 0 2400 2800" style="enable-background:new 0 0 2400 2800;" xml:space="preserve">
        <g>
            <g id="Layer_1-2">
                <path class="st0" d="M500,0L0,500v1800h600v500l500-500h400l900-900V0H500z M2200,1300l-400,400h-400l-350,350v-350H600V200h1600
                    V1300z"/>
                <rect x="1700" y="550" class="st0" width="200" height="600"/>
                <rect x="1150" y="550" class="st0" width="200" height="600"/>
            </g>
        </g>
        </svg>
    </a>
</div>

<style>
    svg {
        width: 24px;
        height: 24px;
        fill: #ffffff;
    }

    .twitch-logo {
        padding: 0 15px;
    }
</style>