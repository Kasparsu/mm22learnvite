<script>
    let people = [
        {name: 'Some name1', text: 'Some text1', img:'https://picsum.photos/seed/people1/350/500?grayscale&blur=10'},
        {name: 'Some name2', text: 'Some text2', img:'https://picsum.photos/seed/people2/350/500?grayscale&blur=10'},
        {name: 'Some name3', text: 'Some text3', img:'https://picsum.photos/seed/people3/350/500?grayscale&blur=10'},
        {name: 'Some name4', text: 'Some text4', img:'https://picsum.photos/seed/people4/350/500?grayscale&blur=10'},
        {name: 'Some name5', text: 'Some text5', img:'https://picsum.photos/seed/people5/350/500?grayscale&blur=10'},
        {name: 'Some name6', text: 'Some text6', img:'https://picsum.photos/seed/people6/350/500?grayscale&blur=10'},

    ];
</script>


<div class="container-fluid my-5">
    <div class="container text-center my-5">
      <h1>Teamwork makes the dream works</h1>
    </div>
    <div class="row">
      {#each people as person}  
        <div class="col-2">
            <div class="card border-0">
            <img src={person.img} class="card-img-top rounded-0" alt="...">
            <div class="card-body text-center">
                <h5 class="card-title">{person.name}</h5>
                <p class="card-text">{person.text}</p>
            </div>
            </div>
        </div>
      {/each}
    </div>
  </div>