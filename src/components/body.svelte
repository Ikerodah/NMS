<script>
    import Thumbnail from "./thumbnail.svelte"
    import Banner1 from "./banner1.svelte"

    let banner = {
        "1":{"quote":`"Through teaching, guiding and mentoring, <br>each child is set on a path to reach their highest potential"`,"buttonText":`Join Us Today`}
    }
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

        <Thumbnail title="About" image = "i11.jpg" />
        <Thumbnail title="Gallery" image="i11.jpg"/>

        <Thumbnail title="Admission" image="i11.jpg" />
        <Thumbnail title="News" image="i11.jpg" />

        <Thumbnail title="Academics" image="i11.jpg" />
        <Thumbnail title="contact" image="i11.jpg" />
    </div>
    <div class="advertise h-32 bg-gray-900">
        <Banner1 quote={banner[1].quote} buttonText={banner[1].buttonText}/>

    </div>
    <div class="socials h-64 bg-gray-900 w-full"></div>
</div>
