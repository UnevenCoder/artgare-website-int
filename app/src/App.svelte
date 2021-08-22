<script>
  let example_obj = [
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_8b0a30abd6ff44caa77c7e77e6edf20c~mv2.png/v1/fill/w_383,h_216,al_c,q_85,usm_0.66_1.00_0.01/6b39b9_8b0a30abd6ff44caa77c7e77e6edf20c~mv2.webp",
      model_name: "Retro Radio",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_f28ecda23802443aa2fe30983e53a4ce~mv2.png/v1/fill/w_383,h_216,al_c,q_85,usm_0.66_1.00_0.01/6b39b9_f28ecda23802443aa2fe30983e53a4ce~mv2.webp",
      model_name: "Sofa/Couch",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_848a72ca6ad548d19dbc7ed13b7b3430~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_848a72ca6ad548d19dbc7ed13b7b3430~mv2.webp",
      model_name: "Wooden Fence",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_d94bad8b85f5426c85a3c89f5ee5f5d1~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_d94bad8b85f5426c85a3c89f5ee5f5d1~mv2.webp",
      model_name: "Toilet Seat",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_1351698db5e14f588ef0640119a0daf4~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_1351698db5e14f588ef0640119a0daf4~mv2.webp",
      model_name: "bomb",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_89973196e65e4d769686b766519a374b~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_89973196e65e4d769686b766519a374b~mv2.webp",
      model_name: "Hammer",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_8b0a30abd6ff44caa77c7e77e6edf20c~mv2.png/v1/fill/w_383,h_216,al_c,q_85,usm_0.66_1.00_0.01/6b39b9_8b0a30abd6ff44caa77c7e77e6edf20c~mv2.webp",
      model_name: "Retro Radio",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_d94bad8b85f5426c85a3c89f5ee5f5d1~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_d94bad8b85f5426c85a3c89f5ee5f5d1~mv2.webp",
      model_name: "Toilet Seat",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_1351698db5e14f588ef0640119a0daf4~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_1351698db5e14f588ef0640119a0daf4~mv2.webp",
      model_name: "bomb",
    },
    {
      model_image:
        "https://static.wixstatic.com/media/6b39b9_89973196e65e4d769686b766519a374b~mv2.jpg/v1/fill/w_383,h_216,al_c,q_80,usm_0.66_1.00_0.01/6b39b9_89973196e65e4d769686b766519a374b~mv2.webp",
      model_name: "Hammer",
    },
  ];
</script>

<main>
  <section id="showcase">
    {#each example_obj as model}
      <div class="box" style="background-image:url({model.model_image})">
        {model.model_name}
      </div>
    {/each}
  </section>
</main>

<style>
  main {
    width: 100vw;
    height: max-content;
    display: flex;
    justify-content: center;
  }
  #showcase {
    width: 80vw;
    min-height: 400px;
    max-height: 800px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: 1fr 1fr 1fr;
    gap: 20px 20px;
  }
  .box {
    width: 100%;
    height: 150px;
    border-radius: 3px;
    border: solid 1px #707070;
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }
  .box:hover {
    border-radius: 5px;
    border: solid 3px red 15ms;
  }
</style>
