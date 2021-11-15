<script>
    import Thumbnail from "./thumbnail.svelte"
    import Banner1 from "./banner1.svelte"
</script>

<div>
    <!-- <div class="bg-yellow-400 h-1"></div> -->
    <div class="bg-yellow-500 h-1"></div>

    <div class="bg-gray-800 h-1"> </div>
    <div class="advertise h-32 bg-gray-900">
    </div>
    <div class="advertise h-10 bg-gray-900">
    </div>
    <div class="advertise h-32 bg-gray-900">
        <Banner1 />
    </div>

    <div class="bg-gray-900 h-auto p-36 pt-16 pb-10 grid grid-rows-2 grid-flow-col gap-4"> 

        <Thumbnail />
        <Thumbnail />
        <Thumbnail />

        <Thumbnail />
        <Thumbnail />
        <Thumbnail />
    </div>
    <div class="advertise h-32 bg-gray-900">
        <Banner1 />

    </div>
    <div class="socials h-64 bg-gray-900 w-full"></div>
</div>
