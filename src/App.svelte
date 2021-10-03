<script>
  import Navbar from "./Navbar.svelte";
  import TrendCard from "./TrendCard.svelte";
  import Footer from "./Footer.svelte";
  import TrendsTable from "./TrendsTable.svelte";
</script>

<main>
  <Navbar />
  <div class="row">
    <TrendCard />
    <TrendsTable />
  </div>

  <Footer />
</main>

<style>
  /* Paper CSS imports */
  @import url("https://unpkg.com/papercss@1.8.2/dist/paper.css");
  @import url("https://unpkg.com/papercss@1.8.2/dist/paper.min.css");
  @import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css")
</style>
