<script>
    
</script>


<div id="container">

    <div id="search_bar">
        <i id="icon" class="fas fa-search"></i>
        <input id="input_field" type="text" placeholder="Search the Web...">
    </div>
</div>

<style>
    #container {
        display: flex;
        justify-content: center;
        flex-direction: column;

        width: 100%;
        max-width: calc(750px + 2em);
        margin: 0px 30px;

        border: 1px solid transparent;
        border-radius: 10px;
        background-color: var(--sbg);
        box-shadow: 0px 0px 3px 0px var(--shadow);
    }

    #search_bar {
        display: flex;
        align-items: center;
        justify-content: center;

        width: 100%;
        height: 100%;
        max-height: 2.5em;

        background-color: transparent;
    }

    #icon {
        font-size: 20px;
        margin: 10px;
        opacity: 50%;

        background-color: transparent;
    }

    #input_field {
        width: 100%;
        height: 100%;

        padding: 10px 20px 10px 5px;

        border: none;
        background: none;
        outline: none;
    }

</style>
