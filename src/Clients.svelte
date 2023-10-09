<script>
    let logos = [
        'https://picsum.photos/seed/logo1/80/80?grayscale&blur=10',
        'https://picsum.photos/seed/logo2/80/80?grayscale&blur=10',
        'https://picsum.photos/seed/logo3/80/80?grayscale&blur=10',
        'https://picsum.photos/seed/logo4/80/80?grayscale&blur=10',
        'https://picsum.photos/seed/logo5/80/80?grayscale&blur=10',
        'https://picsum.photos/seed/logo6/80/80?grayscale&blur=10',
    ];
</script>
<div class="container-fluid p-0">
    <div class="row">
      <div class="col-6 d-flex align-items-center bg-secondary-subtle p-0">
        <div class="container mx-5 px-5">
          <h1>Company Clients</h1>
          <p class="text-secondary fw-semibold">
            We work with clients from all over the world.
            We had worked with and serving over 2000 customers and 1000 global companies across
            13 countries with over 90% satisfaction rate achieved.
          </p>
          <button class="btn">Learn more</button>
        </div>
      </div>
      <div class="col-6 p-0">
          <div class="row px-5 pt-5 mb-5">
            {#each logos as logo}
                <div class="col-4 px-5 mb-5"><img class="w-100" src={logo}></div>
            {/each}
          </div>
      </div>
    </div>
  </div>