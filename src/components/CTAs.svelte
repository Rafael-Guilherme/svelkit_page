<script lang="ts">
    export let dark: Boolean;
</script>

<div class="flex items-center gap-4">
    <button class={"specialBtn " + (dark ? " bg-[#181b34]" : " ")}>
        <p class="text-base sm:text-lg md:text-xl">Entre em contato</p>
    </button>
    <button class="specialBtnDark">
        <p class="text-base sm:text-lg md:text-xl">Comece agora &rarr;</p>
    </button>
</div>