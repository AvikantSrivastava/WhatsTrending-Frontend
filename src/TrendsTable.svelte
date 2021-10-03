<script>
  let dataPromise = getData();

  async function getData() {
    return fetch("https://twitter-trends-daily.herokuapp.com/alltrends").then(
      (response) => {
        return response.json();
      }
    );
  }
</script>

<div class="sm-12 md-4 col sidebar">
  <div class="paper">
    <h3>
      <center>Other locations</center>
    </h3>
    <div>
      <table id="TrendsTable" />
      {#await dataPromise}
        loading
      {:then data}
        {#each Object.entries(data.trends) as [location, trends]}
          {#if location != "key"}
            <div class="collapsible">
              <input
                id="collapsible{location}"
                type="checkbox"
                name="collapsible"
              />
              <label for="collapsible{location}">{location}</label>
              <div class="collapsible-body">
                <ol
                  style="display: inline-block text-align:left; list-style-position: inside;"
                >
                  {#each trends as trend}
                    <li>
                      <a href="https://twitter.com/search?q={trend}">{trend}</a>
                    </li>
                  {/each}
                </ol>
              </div>
            </div>
          {/if}
        {/each}
      {/await}
    </div>
  </div>
</div>