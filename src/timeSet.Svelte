<script>
   export let time = {
        workTime: 0,
        breakTime: 0,
    };
</script>

<div>
    <button
        on:click={() => {
            time.workTime += 5;
        }}
    >
        &bigtriangleup;</button
    >
    <br />
    <h2>{time.workTime} mins</h2>
    <br />
    <button
        on:click={() => {
            !time.workTime ? time.workTime : (time.workTime -= 5);
        }}
    >
        &bigtriangledown;
    </button>
</div>

<div>
    <button
        on:click={() => {
            time.breakTime += 5;
        }}
        disabled=""
    >
        &bigtriangleup;</button
    >
    <br />
    <h2>{time.breakTime} mins</h2>
    <br />
    <button
        on:click={() => {
            !time.breakTime ? time.breakTime : (time.breakTime -= 5);
        }}
    >
        &bigtriangledown;
    </button>
</div>

<style>
    div {
        margin: 0 30px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>
