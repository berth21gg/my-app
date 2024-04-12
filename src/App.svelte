<script>
  import Button from "./components/Button.svelte";
  import Text from "./components/Text.svelte";
  import Input from "./components/Input.svelte";
  import Photos from "./components/Photos.svelte";

  let name = "Bernardo"

  const info = {
    nombre: 'Bernardo',
    apellido: 'Tierranegra',
    edad: 23,
  }

</script>

<main>
  <h1>Hello { name }</h1>
  <Button />
  <Text {...info} />
  <Text nombre={info.nombre} apellido={info.apellido} edad={info.edad}/>
  <Input />
  <Photos />
</main>


<style>
  :global(body){
    background-color: #f2eee2;
    color: #0084f6;
    transition: background-color 300ms, color 300ms;
  }

  :global(body.dark-mode){
    background-color: #1d3040;
    color: #bfc2c7;
    transition: background-color 300ms, color 300ms;
  }

  main{
    text-align: center;
  }

  h1{
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

</style>