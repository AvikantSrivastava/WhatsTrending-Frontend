<script>
  let developer = {
    name: "Avikant Srivastava",

    socialMedia: {
      linkedin: {
        link: "https://www.linkedin.com/in/avikantsrivastava/",
        profile: "Avikant Srivastava",
      },
      github: {
        link: "https://github.com/avikantsrivastava",
        profile: "@AvikantSrivastava",
      },
      twitter: {
        link: "https://twitter.com/aestheticell",
        profile: "@Aesthetixell",
      },
      instagram: {
        link: "https://www.instagram.com/aesthetixell/",
        profile: "@Aesthetixell",
      },
    },
  };
</script>

<div class="card-footer">
  <div class="paper container container-md margin-bottom-large card">
    <div class="card-body">
      <center>
        <h3 class="card-title">
          Made with <span style="color: #e25555;">&#9829;</span> by <br />
          {developer.name}
        </h3>
      </center>
    </div>
    <div class="row flex-spaces">
        <center>
          {#each Object.entries(developer.socialMedia) as [name, socialMedia]}
            <h5 class="card-subtitle">
              <a href={socialMedia.link}
                ><i class="fa fa-{name}" />  {socialMedia.profile}</a
              >
            </h5>
          {/each}
        </center>
    </div>
  </div>
</div>
