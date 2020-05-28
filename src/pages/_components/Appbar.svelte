<div>
    <h1>ProblemX</h1>
    <div class="typewriter">
        <p>A website full of problems ...</p>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Inconsolata:wght@400;500&display=swap');

    div {
        color: white;
        text-align: center;
        font-family: "Inconsolata", monospace;
        font-size: 25px;
    }

    .typewriter {
        width: 90%;
        margin: 0 auto;
    }

    .typewriter p {
        border-right: solid 2px white;
        white-space: nowrap;
        overflow: hidden;
        animation: type-text 4s linear 1s 1 normal both,
        type-cursor 600ms linear infinite;
        font-size: 20px;
    }

    @keyframes type-text {
        from{width: 0}
        to{width: 100%}
    }

    @keyframes type-cursor {
        from{border-right-color: white}
        to{border-right-color: transparent}
    }

    @media screen and (min-width: 800px) {
        .typewriter {
            width: 25%;
            margin: 0 auto;
        }

        .typewriter p {
            font-size: 25px;
        }
    }

    :global(body) {
        background-color: #2C2F33;
    }
</style>