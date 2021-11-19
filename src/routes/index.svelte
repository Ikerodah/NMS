<!-- <div class="h-[800px] bg-blue-200">
    <div class="flex h-80 px-12 py-8 flex items-end" >
        <div class="box1 box m-2 bg-gray-900 h-full w-6/12 hover:scale-105">Box 1</div>
        <div class="box2 box m-2 bg-white w-5/12 h-5/6">Box 2</div>
        <div class="w-1/12"></div>
    </div>

    <div class="flex h-80 mx-10">
        <div class="box3 box m-2 bg-gray-900 h-full w-6/12">Box 1</div>
        <div class="box4 box m-2 bg-white w-5/12 h-5/6">Box 2</div>
        <div class="w-1/12"></div>
    </div>

</div> -->
<script>
const box1 = `m-2 bg-green-900 h-full w-6/12`
let box1_live = box1

let scale_105 = `scale-105`
const ffadd = () => {
    box1_live = `${box1} ${scale_105}`
    setTimeout(ffremove,3000)

}
const ffremove = () => {
    box1_live = box1
    setTimeout(ffadd,2000)

}

setTimeout(ffadd,2000)


</script>


<div class="h-[800px] bg-blue-200">
    <button class="m-2 bg-blue-600 text-white px-6 py-2 rounded-md" on:click="{ffadd}">
        Add
    </button>
    <button class="m-2 bg-red-600 text-white px-6 py-2 rounded-md" on:click="{ffremove}">
        Remove
    </button>
    
    <div class="flex h-80 px-12 py-4 flex items-end" >
        <div class="{box1_live} hover:scale-105 transition duration-500">Box 1</div>
        <div class="box2 box m-2 bg-white w-5/12 h-5/6">Box 2</div>
        <div class="w-1/12"></div>
    </div>

    <div class="flex h-80 mx-10">
        <div class="box3 box m-2 bg-gray-900 h-full w-6/12">Box 1</div>
        <div class="box4 box m-2 bg-white w-5/12 h-5/6">Box 2</div>
        <div class="w-1/12"></div>
    </div>

</div>

<style>
    .box:hover{
        background-color: #550f2c;
        transition-duration:1s;
    }
    .test{
        background-color: green;
    }

</style>