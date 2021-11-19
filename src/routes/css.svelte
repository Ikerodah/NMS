

<script>
    

let name = "Green"
    let _original = `box1 my-4 rounded-md bg-blue-500 h-32 w-1/6 transition duration-500`
    let _scaled = `box1 my-4 rounded-md bg-green-500 h-32 w-1/6 scale-105 transition duration-500`
    let trigger = true
    let _class = _original



let mtfunc = () => {
    if (trigger)
        _class =_scaled
    else 
        _class = _original

    trigger = !trigger
}



setInterval(mtfunc, 4000)

</script>
<div class="p-10 h-screen bg-yellow-100">
    <button class=" {trigger?"bg-red-600":"bg-pink-400"} text-white px-10 py-3 rounded-md" on:click="{mtfunc}">Trigger</button>

    <div class={`${_class}`}></div>

</div>


<style>
 

</style>
