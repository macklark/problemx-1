<script>
    let title = "";
    let desc = "";
    let category = ""
    const create_problem = () => {
        console.log(title)
    }
</script>

<main>
<div id = "cards">
    <form on:submit|preventDefault = {create_problem}>
    <div id = "head">
        <h1>Create a problem</h1>
    </div>
    <div id = "wrapper">
        <div id = "card">
            <label>Title</label>
                <input  type = "text" required bind:value = {title}>
            </div>

        <div id = "card">
            <label>Description</label>
            <textarea type = 'text' rows = "5" cols = "35"  required bind:value = {desc}></textarea>
        </div>

    <div id = "card">
            <label>Categories</label>
            <input type = "text" required bind:value = {category} placeholder = "Enter Comma Seperated Values">
    </div>

    </div>

    <div id = "btn">
        <button>
            Submit
        </button>
    </div>

    </form>
</div>

</main>

<style>
    form{
        color: white;
        text-align: center;
        font-size: 18px
    }

    #card{
        margin: 30px;
        /* text-align: center */
    }

    textarea{
        margin : 8px;
        background-color: lightgray;
        width : 100%;
        margin-left: auto;
        margin-right: auto
    }


    input{
        margin: 8px;
        width : 100%;
        background-color: lightgray;
        margin-left: auto;
        margin-right: auto
    }

    input:focus{
        outline: none
    }


    button{
        margin: 10px;
        padding : 10px;
        padding-left: 35px;
        padding-right: 35px
    }

    #wrapper{
        margin: 30px
    }

    button:hover{
        cursor: pointer;
    }

    textarea:focus{
        outline: none
    }


    @media screen and (min-width: 760px){
        input{
            width : 40%
        }

        textarea{
            width : 40%
        }
    }
</style>
