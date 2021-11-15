<script>
    import Badge from "./badge.svelte"
    import Navigation from "./navigation.svelte"

</script>


<div class="flex items-end h-auto customfade  pb-1 pt-0 ">
    <div class="w-1/2  ">
        <Badge />
    </div>
    <div class="w-1/2 mb-5 h-full ">
        <Navigation />
    </div>
</div>

<style>
    .customfade{
        background: hsla(48, 100%, 96%, 1);

/* background: linear-gradient(90deg, hsla(48, 100%, 96%, 1) 13%, hsla(48, 100%, 96%, 0.95) 100%);

background: -moz-linear-gradient(90deg, hsla(48, 100%, 96%, 1) 13%, hsla(48, 100%, 96%, 0.95) 100%);

background: -webkit-linear-gradient(90deg, hsla(48, 100%, 96%, 1) 13%, hsla(48, 100%, 96%, 0.95) 100%); */

    }
</style>