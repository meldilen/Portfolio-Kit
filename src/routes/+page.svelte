<script>
    import penguin from '$lib/images/pngwing.com(1).png';
</script>

<div>
    <img src={penguin} alt = "My logo penguin!" class = "logo">
    <h1>DZIYANA MELNIKAVA</h1>
    <p class = "quote">-Is it working? Don't touch.</p>
    <p class = "author">Any programmer</p>
</div>

<style>
    p{
        background-color:dimgrey;
        font-size: 20px; 
        padding-left: 1%;
        padding-right: 1%;
        color:rgb(255, 255, 255); 
    }
    .author
    {
        position: absolute; 
        top:63%; 
        font-style: italic;
        left: 72%;
    }
    .quote
    {
        position: absolute; 
        top:58%; 
        left: 60%;
    }
    .logo
    {
        position: absolute; 
        top:52.5%; 
        left:27%; 
        width: 19.5%;
    }
    h1
    {
        font-family: serif; 
        font-style: italic; 
        font-size: 100px; 
        color:rgb(73, 72, 72); 
        position: absolute; 
        top:20%; 
        left: 53%
    }
</style>