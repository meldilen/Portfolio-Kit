<script>
    import {base} from "$app/paths";
</script>
<header>
    <nav>
        <ul class = "navigation_class">
            <li><a href="{base}/folder">HOME PAGE</a>
            <li><a href="https://github.com/meldilen?tab=repositories">PROJECTS</a>
            <li><a href="{base}/">PENGUIN</a>
        </ul>
    </nav>
</header>

<style>
    header
    {
        background-color:dimgrey; 
        height:10vh;
    }
    ul.navigation_class
    {
        display: flex; 
        right:10%;
        position: absolute;
        list-style: none; 
        top: 1%;
    }
    .navigation_class li a
    {
        margin: 20px;  
        color:white; 
        text-decoration: none; 
        cursor: pointer; 
        font-size:25px;
    }
</style>
