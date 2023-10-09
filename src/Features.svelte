<script>
    let features = [
        {
            title: 'Modern Design',
            text: 'Brook embraces a modern look with various enhanced pre-defined page elements.',
            img: '\\home-design-studio-image-01.png'
        },
        {
            title: 'Multi-purpose Use',
            text: 'This is the theme for businesses & companies operating in a wide range of areas.',
            img: '\\home-design-studio-image-02.png'
        },
        {
            title: 'Responsive Design',
            text: 'Brook is highly responsive thanks to built-in WPBakery Page Builder & Slider Revolution plugins.',
            img: '\\home-design-studio-image-03.png'
        }
    ]
</script>

<div class="container-fluid bg-danger-subtle">
    <div class="container text-center ">
      <h1>Best services save the world</h1>
      <div class="row py-5">
        {#each features as feature}
            <div class="col">
                <div class="card h-100 border-0">
                    <img src={feature.img} style="width:120px" class="card-img-top mx-auto mt-2" alt="...">
                    <div class="card-body">
                    <h5 class="card-title">{feature.title}</h5>
                    <p class="card-text">{feature.text}</p>
                    <a href="#" class="btn fw-bold">More details</a>
                    </div>
                </div>
            </div>
       {/each}
      </div>

      <div class="row">
        <div class="col-6 offset-3">
          <p class="text-secondary fw-semibold">Since its establishment in 2000, Brook Creative has been focusing on project management & implementation through global cooperation & partners.</p>
          <button class="btn btn-danger fw-bold btn-lg my-3">Learn More</button>
        </div>
      </div>
    </div>
  </div>