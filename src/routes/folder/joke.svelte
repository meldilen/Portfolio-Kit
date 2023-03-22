<script lang="ts">
    import { onMount } from "svelte";
    interface joke_information {
        img: string;
        alt: string;
        title: string;
        year: string;
        month: string;
        day: string;
    }

    let image_discription : {joke?: string, content?: string, isDownloaded?: boolean} = {}

    onMount(async () => {
        const params = new URLSearchParams({
            email: "d.melnikava@innopolis.university"
        });

        const response = await fetch(`https://fwd.innopolis.app/api/hw2?${params.toString()}`);
        const received_id = await response.text();
        const jokeResponse = await fetch(`https://getxkcd.vercel.app/api/comic?num=${received_id}`);
        const data: joke_information = await jokeResponse.json();

        image_discription = {
            content: `${data.title} ${data.day}.${data.month}.${data.year}`,
            joke: data.img, 
            isDownloaded: true
        }

    })
</script>

<br>
<div class="jokeImg">
  <img src={image_discription.joke} alt={image_discription.content} hidden={!image_discription.isDownloaded}>
  <figure>
    <figcaption>{image_discription.content}</figcaption>
  </figure>
</div>

<style>
    .jokeImg {
        width: 27%;
        height: 22%;
        padding-left: 43%;
    }
    .jokeImg figcaption
    {
        color: rgb(0, 0, 0);
        margin-right: 10%;
        float: right;
        font-family: Snell Roundhand, cursive;
    }
</style>