<script > // Add attribute called modules: Special Script
  
  let guides = [];

  let getPosts = async() => {
    const res = await fetch("https://jsonplaceholder.typicode.com/posts");
    const data = await res.json();
    guides = data;
  }

  getPosts();

</script>


<div class="guides">
    <ul>
      {#each guides as guide}
        <li><a href="/">Guide {guide.title}</a></li>  
      {/each}
    </ul>
  </div>
  
  <style>
    .guides {
      margin-top: 20px;
    }
    ul {
      list-style-type: none;
      padding: 0;
    }
    a {
      display: inline-block;
      margin-top: 10px;
      padding: 10px;
      border: 1px dotted rgba(255,255,255,0.2);
    }
  </style>