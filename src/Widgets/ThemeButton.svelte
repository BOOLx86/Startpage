<script>
    let icon_class = 'far fa-moon'

    /* if theme was never saved, set default theme (light) */
    let theme = localStorage.getItem('theme') || 'light';

    apply_theme();

    function toggle_theme() {
        theme = (theme == 'light')? 'dark' : 'light';
        localStorage.setItem('theme', theme);

        apply_theme();
    };

    function apply_theme() {
        switch (theme) {
            case 'dark':
                document.body.classList.add('dark_theme');
                icon_class = 'far fa-sun';
                break;

            case 'light':
                document.body.classList.remove('dark_theme');
                icon_class = 'far fa-moon';
                break;
        
            default:
                break;
        }
    }

</script>


<i on:click="{toggle_theme}" id="theme_button" class={icon_class}></i>

<style>
    #theme_button {
        position: absolute;
        top: 0;
        right: 0;
        margin: 1em;

        font-size: 30px;
    }
    
</style>
