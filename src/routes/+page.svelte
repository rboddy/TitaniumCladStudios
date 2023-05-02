<script>

    let state = true;

    function spin() {
        if(state){
            gsap.to(".titanium-box", {rotation: 360, borderRadius: "45%", duration: 1});
        }
        else {
            gsap.to(".titanium-box", {rotation: -360, borderRadius: "0%", duration: 1});
        }
        state = !state;
    }
</script>

<div class="page-container">
    <div class="titanium-box" on:click={spin}>
        <div class:display={!state}>
            <p>22</p>
            <p>47.867</p>
        </div>
        <div class:display={!state}>
            <h1>Ti</h1>
        </div>
        <div class:display={!state}>
            <p>Titanium</p>
        </div>
    </div>
</div>

<style>
    :global(body){
        margin: 0;
        font-family: 'Roboto', sans-serif;
        /* CSS HEX */
        --black: #000000ff;
        --violet-jtc: #502f4cff;
        --chinese-violet: #70587cff;
        --thistle: #c8b8dbff;
        --snow: #f9f4f5ff;
    }
    .page-container {
        background: #000;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
    }
    .titanium-box {
        width: 32vmin;
        height: 32vmin;
        background-color: #F9F4F5;
        display: grid;
        grid-template-rows: 1fr 2fr 1fr;
        padding: 2vmin;
        box-sizing: border-box;
        font-size: 20px;
        box-shadow: 0 0 50px 15px #70587C;
        color: #502F4C;
        
    }
    .titanium-box > div {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .titanium-box > div:first-child {
        justify-content: space-between;
    }
    .titanium-box:hover {
        cursor: pointer;
    }
    .display {
        display: none !important;
    }
    h1 {
        margin: 0;
        font-size: 4rem;
        font-weight: bold;
    }
    @media(max-width: 480px){
        .titanium-box {
            width: 30vmax;
            height: 30vmax;
        }
        .titanium-box:hover {
            width: 31vmax;
            height: 31vmax;
        }
    }
</style>