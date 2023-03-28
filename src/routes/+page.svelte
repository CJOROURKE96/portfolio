<script>
    import Button from '@smui/button'
    import GoMarkGithub from 'svelte-icons/go/GoMarkGithub.svelte'    
let clicked = 0;
</script>

<div class="sideNav">
    <a class="projectsNav" href="/projects">Projects</a>
    <a class="cvButton" href="src/cv/ConnorORourkeCV.pdf" download="">CV</a>
    <Button 
    on:click={() => clicked++}
    varient="unelevated"
    class="button"
    style="padding: 0; min-width: 32px"
    >
        <div class="icon">
        <GoMarkGithub />
        </div>
    </Button>
    <Button 
    on:click={() => clicked++}
    varient="unelevated"
    class="button"
    >
        <img src="https://w7.pngwing.com/pngs/887/616/png-transparent-linkedin-icon-linkedin-text-rectangle-logo.png" alt="LinkedIn logo" border=0 aria-hidden="true">
    </Button>
</div>
<main>
<h1>Connor O'Rourke</h1>




    <p>Words</p>
</main>


<style>
    .sideNav{
        height: 100%;
        width: 160px;
        position: fixed;
        z-index: 1;
        top: 0;
        left: 0;
        background-color: royalblue;
        overflow-x: hidden;
        padding-top: 20px;
    }
    .sideNav a {
        padding: 6px, 8px, 6px, 16px;
        text-decoration: none;
        font-size: 25px;
        color: whitesmoke;
        display: block;
    }
    main {
        margin-left: 160px;
        padding: 0px, 10px;
    }
    @media screen and (max-height: 450px) {
        .sideNav {padding-top: 15px;}
        .sideNav a {font-size: 18px;}
    }
    img {
        width: 75%;
    }
     .icon{
        width: 32px;
        height: 32px;
        border-radius: 25px;
        background: #73AD21;
        padding: 20px;     
    }
</style>

