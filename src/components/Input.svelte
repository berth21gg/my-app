<script>
    let name = "world";
</script>

<div class="Input">
    <input type="text" bind:value={name}>
    <p>Hello {name}!</p>
</div>

<style>
    
    .Input{
        margin: 20px;
    }
</style>