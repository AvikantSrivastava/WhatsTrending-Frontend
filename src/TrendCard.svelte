<div class="sm-12 md-8 col">
  <div class="paper container-lg margin-bottom-large">
    <h3>
      Want to know what is trending around you?
      <button
        id="install_button"
        class="float-right"
        style="visibility: hidden;">Install APP</button
      >
    </h3>
    <p>
      <img
        src="images/robo.png"
        alt=""
        class="float-left no-border"
        width="100"
      />
      We tell you the latest trends in realtime.
    </p>
    <p>
      Our Algorithm looks for people's reaction on Twitter on different trends,
      based on <b>Machine Learning</b> it tells you how Positive or Negative the
      trend is.
    </p>

    <div class="row flex-spaces tabs">
      <input id="tab1" type="radio" name="tabs" checked />
      <label for="tab1">
        <h3>India</h3>
      </label>

      <input id="tab2" type="radio" name="tabs" />
      <label for="tab2">
        <h3>World</h3>
      </label>

      <div class="content" id="content1">
        <center>
          <table id="contentIndia" style="text-align:center;" />
        </center>
      </div>

      <div class="content" id="content2">
        <table id="contentWorld" style="text-align:center;" />
      </div>
    </div>
  </div>
</div>
