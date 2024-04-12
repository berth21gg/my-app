<script>

let styles = { darkMode: false}

function toggle(){
    styles.darkMode = !styles.darkMode;
    window.document.body.classList.toggle("dark-mode");
}

</script>

<div class="Button">
        
    <button on:click={toggle}>{styles.darkMode ? 'LightMode🌞' : 'DarkMode🌒'}</button>

</div>

<style>

    button {
        border-radius: 8px;
        border: 1px solid transparent;
        padding: 0.6em 1.2em;
        font-size: 1em;
        font-weight: 500;
        font-family: inherit;
        background-color: #6c8ca4;
        cursor: pointer;
        transition: border-color 0.25s;
    }   
</style>