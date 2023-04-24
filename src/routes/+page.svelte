<div class="page-container">
    <div class="titanium-box">
        <div>
            <p>22</p>
            <p>47.867</p>
        </div>
        <div>
            <h1>Ti</h1>
        </div>
        <div>
            <p>Titanium</p>
        </div>
    </div>
</div>

<style>
    :global(body){
        margin: 0;
        font-family: 'Roboto', sans-serif;
    }
    .page-container {
        background: #000;
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100vh;
    }
    .titanium-box {
        width: 30vmin;
        height: 30vmin;
        background-color: #F9F4F5;
        display: grid;
        grid-template-rows: 1fr 2fr 1fr;
        padding: 2vmin;
        box-sizing: border-box;
        border-radius: 5px;
        font-size: 20px;
        box-shadow: 0 0 50px 15px #70587C;
        color: #502F4C;
    }
    .titanium-box:hover {
        width: 31vmin;
        height: 31vmin;
    }
    .titanium-box > div {
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .titanium-box > div:first-child {
        justify-content: space-between;
    }
    h1 {
        margin: 0;
        font-size: 4rem;
        font-weight: bold;
    }
</style>