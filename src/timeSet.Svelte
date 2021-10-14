<script>

    let num = 0;

    function addTime() {
        num += 5;
    }

    function subTime() {
        if (num !== 0) {
            num -= 5;
        } else {
            num = 0;
        }
    }
</script>

<div>
    <button on:click={addTime}> &bigtriangleup;</button> 
    <br>
    <h2> {num} mins</h2>
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
