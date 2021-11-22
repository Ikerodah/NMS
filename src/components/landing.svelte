<script>
    let box1,box2,box3,box4
    box1=box2=box3=box4=""

    let box_scale = `scale-105`

const ffanimate = () =>{
        box1 = box_scale
        setTimeout(()=>{
            box4 = box_scale
            setTimeout(()=>{
                box4=""
                box1 =""
                box2=box_scale
                setTimeout(()=>{
                    box3=box_scale
                    setTimeout(()=>{
                        box3=""
                        box2=""
                        ffanimate()
                    },10000)
                },10000)
            },9000)
        },10000)
}
ffanimate()





</script>


<!-- <div class="clear-right bg-yellow-50 bg-opacity-90 "> --> 
<div class="clear-right customfade ">

    <div class="flex h-80 px-36 pt-4 items-end" >
        <div class="{box1}  cursor-pointer box1 shadow-2xl m-2 h-full w-6/12 bg-cover hover:scale-105 transition duration-700 rounded-xl" style="background-image: url(../static/test/erste3.png) ">
            <!-- <img class="h-full w-full" src="sel_1.jpg" alt=""> -->
            <!-- <div class=" h-full bg-blue-700 bg-opacity-0 hover:bg-opacity-40 transition-all duration-300"></div> -->

        </div>
        <!-- <div class="box2 m-2 mt-0 h-5/6 w-5/12 bg-cover" style="background-image: url(../static/test/i1_2.jpg)"></div> -->
        <!-- <div class="box2 m-2 mt-0 h-5/6 w-5/12 bg-cover " style="background-image: url(../static/test/i11.jpg)"> -->
            <!-- <div class="box2 m-2 mt-0 h-5/6 w-5/12 bg-cover " style="background-image: url(../static/test/04.jpg)"> -->
                <div class="{box2} box2 m-2 mt-0 h-5/6 w-5/12 bg-cover shadow-2xl hover:scale-105 transition duration-700 cursor-pointer rounded-xl" style="background-image: url(../static/test/dreite2.png)">


        </div>

    </div>

    <div class="flex h-32 px-36 ">
        <div class="w-2/12"></div>
        <!-- <div class="box3 mr-2 mt-2 h-60 w-5/12 bg-cover " style="background-image: url(../static/test/i21.jpg)"></div> -->
        <div class="{box3} box3 shadow-2xl mr-2 mt-2 h-60 w-5/12 bg-cover hover:scale-105 transition-all duration-500 cursor-pointer rounded-xl" style="background-image: url(../static/test/sexte.png)"></div>

        <!-- <div class="box4 ml-2 mt-2 h-60 w-5/12 bg-cover" style="background-image: url(../static/test/i19.jpg) "></div> -->
        <div class="{box4} box4 ml-2 mt-2 shadow-2xl h-60 w-5/12 bg-cover hover:scale-105 transition-all duration-500 cursor-pointer rounded-xl" style="background-image: url(../static/test/zweite9.png) "></div>

    </div>
</div>


<style>
    .customfade{
        background: hsla(48, 100%, 96%, 1);
    }
</style>