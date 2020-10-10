<style>
h3 {
  margin-bottom: 15px;
}
h4::before {
	content: '> ';
}
h5::before {
  font-family: "Font Awesome 5 Free";
  content: '\f07c';
  font-size: 15px;
  margin-right: 5px;
  margin-left: 5px;
  }
img {
  max-width: 200px;
  box-shadow: 15px 15px #000;
}
summary {
  cursor: pointer;
  outline: none;
  height: 20px;
}
summary::-webkit-details-marker {
  display: none;
}
@media (max-width:480px) {
  .container {
    flex-wrap: wrap !important;
  }

  .item {
      width: 100% !important;
  }
}
.container {
  display: flex;
  margin-top: 20px;
  width: 100%;
}
.item {
  width: 50%;
}
.about-h2 {
  font-size: 24px;
  width: fit-content;
  color: #fff;
  border: 2px solid #fff;
	padding-top: 6.125px;
	padding-bottom: 7px;
	padding-left: 10.5px;
	padding-right: 11.5px;
}
.profile {
  margin-top: 20px;
}
.profile-resume {
  margin: 10px 0;
}
.profile-text {
  margin-top: 15px;
}
.profile-text-description {
  margin-bottom: 5px;
	color: #55FF55
}

.tree {
  margin-top: -18px;
}
.tree, .tree ul, .tree li {
  position: relative;
  color: #fff;
}
.tree ul {
  list-style: none;
  padding-left: 24px;
}
.tree li::before, .tree li::after {
  content: "";
  position: absolute;
  left: -12px;
}
.tree li::before {
  border-top: 2px solid #fff;
  top: 9px;
  width: 8px;
  height: 0;
}
.tree li::after {
  border-left: 2px solid #fff;
  height: 100%;
  width: 0px;
  top: 2px;
}
.tree ul > li:last-child::after {
    height: 8px;
}
</style>

<svelte:head>
	<title>About</title>
</svelte:head>

<h1>About me</h1>

<div class="container">
  <div class="item">
    <div class="profile">

      <div class="profile-resume">
        <h2 class="about-h2">profile</h2>
      </div>

      <img src="./image/me.png" alt="me">

      <div class="profile-text">
        <h3>Resume</h3>
        <h4>Name</h4>
        <p class="profile-text-description">Ocat</p>
        <h4>Location</h4>
        <p class="profile-text-description">Tokyo/Japan</p>
        <h4>Email</h4>
        <p class="profile-text-description">catjp@protonmail.ch</p>
        <h4>Jobs</h4>
        <p class="profile-text-description">Frontend Engineer</p>
        <h4>Tertiary</h4>
        <p class="profile-text-description">
          Public Management of Economics in KINDAI University<br>
          Higashiosaka City (Osaka Prefecture)<br>
          Batch 2016-2020
        </p>
        <h4>Secondary</h4>
        <p class="profile-text-description">
          Chiben Gakuen Senior High School (Nara Prefecture)<br>
          Participated in the 66th All-Japan High School Ekiden Championship<br>
          Batch 2013-2015
        </p>
      </div>

      <p>The design was inspired by <a href="https://kristopolous.github.io/BOOTSTRA.386/index.html" target=”_blank”>BOOTSTRA.386</a></p>
    </div>
  </div>
  <div class="item">
    <div class="profile">
      <h2 class="about-h2">Knowledge tree structure</h2>
      <div class="tree">
        <ul>
        <!-- from here -->
          <li>
            <details open>
              <summary><h5>Web</h5></summary>
              <ul>

                <li>
                  <details open>
                  <summary><h5>Icons</h5></summary>
                  <!-- <h5>Icons</h5> -->
                  <ul>
                    <li><a href="https://fontawesome.com/">Font Awesome</a></li>
                    <li><a href="https://css.gg/">css.gg</a></li>
                    <li><a href="https://icones.js.org/">Icones</a></li>
                  </ul>
                  </details>
                </li>

                <li>
                  <details open>
                  <summary><h5>Article</h5></summary>
                  <!-- <h5>Icons</h5> -->
                  <ul>
                    <li><a href="https://fontawesome.com/">Font Awesome</a></li>
                    <li><a href="https://css.gg/">css.gg</a></li>
                    <li><a href="https://icones.js.org/">Icones</a></li>
                  </ul>
                  </details>
                </li>

              </ul>
            </details>
          </li>

          <li>
            <details open>
              <summary><h5>TEST</h5></summary>
              <ul>
                <li>Beef</li>
                <li>Pork</li>
              </ul>
            </details>
          </li>
        <!-- So far -->
        </ul>
      </div>
    </div>

  </div>
</div>