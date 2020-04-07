<script>
  let forgedInFire = [
    { id: "FKKeZqe0X7Q", name: "forged in fire charlemagne" },
    { id: "9hSqGq3hM1c", name: "forged in fire javanese kris" },
    { id: "EVhTGmdUkkA", name: "forged in fire zhanmadao" }
  ];
</script>

<h1>i pick some forged in fire episode</h1>

<ul>
  {#each forgedInFire as { id, name }, i}
    <li>
      <a href="https://www.youtube.com/watch?v={id}" target="_blank">
        {i + 1} : {name}
      </a>
    </li>
  {/each}
</ul>
