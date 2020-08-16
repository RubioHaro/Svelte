<script>
  let skills = [
    { id: 1, name: "Sabiduria" },
    { id: 2, name: "Empatia" },
    { id: 3, name: "Fuerza" },
  ];
</script>

<div class="Skills">
  <h3>Habilidades</h3>
  <ul>
    {#each skills as skill, i}
      <li>{skill.name}</li>
    {/each}
  </ul>
</div>

<style>
    .Skills{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    ul{
        margin: 0;
        padding: 0;
        list-style: none;
    }
    li{
        display: inline;
        margin: 0 0 0 0.4rem;
    }
</style>
