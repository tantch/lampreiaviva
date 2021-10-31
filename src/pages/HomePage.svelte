<script>
</script>
<div class="page">
  <div class="main-image">
    <img src="https://apef.pt/wp-content/uploads/2020/05/placeholder.png"/>
  </div>
  <div class="section-title">Clientes</div>
  <div class="carousel">
    {#each [1,2,3,4] as cliente}
      <div class="client">
        <img src="https://apef.pt/wp-content/uploads/2020/05/placeholder.png"/>
      </div>
    {/each}
  </div>
</div>

<style>
  .main-image {
    margin:0 20%;
  }
  .main-image > img {
    width:100%;
  }
  .section-title {
    margin: 150px 0px 80px 0px;
    text-align:center;
  }
  .client {
    width:250px;
    height:100px;
    margin: 0px 20px;
  }
  .client > img {
    width:100%;
  }
</style>
