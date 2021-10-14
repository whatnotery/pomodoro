<script>

    let time = {
        worktime : 0,
        breaktime: 0
     } 

    function addTime(num) {
        num += 5;
    }

    function subTime(num) {
        if (num !== 0) {
            num -= 5;
        } else {
            num = 0;
        }
    }
</script>

<div>
    <button on:click={() => addTime(time.worktime)}> &bigtriangleup;</button> 
    <br>
    <h2> {time.worktime} mins</h2>
    <br>
    <button on:click={subTime}> &bigtriangledown; </button>
</div>


<style>
    div {
        margin: 0 30px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>
