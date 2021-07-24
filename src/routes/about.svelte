<script>
</script>
<style>
h3 {
  margin-bottom: 15px;
}
h4::before {
	content: '> ';
}
img {
  max-width: 200px;
  box-shadow: 15px 15px #000;
}
@media (max-width:480px) {
  .container {
    flex-wrap: wrap !important;
  }

  .item {
    width: 100% !important;
  }

  .profile {
    margin: 10px !important;
  }
}
.container {
  display: flex;
  width: 100%;
  overflow-wrap:  break-word;
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
    margin: 20px;
  }
.profile-resume {
  margin-bottom: 10px;
}
.profile-text {
  margin-top: 15px;
}
.profile-text-description {
  margin-bottom: 5px;
	color: #55FF55
}
.profile-text-description-history {
  padding: 4px;
  border: 2px solid #55FF55;
	color: #55FF55
}
</style>

<svelte:head>
	<title>About</title>
</svelte:head>


<div class="container">
  <div class="item">
    <div class="profile">

      <div class="profile-resume">
        <h2 class="about-h2">profile</h2>
      </div>

      <img src="./image/me.png" alt="me">

      <div class="profile-text">
        <!-- <h3>Resume</h3>
        <h4>Name</h4>
          <p class="profile-text-description">Ocat</p>
        <h4>Location</h4>
          <p class="profile-text-description">Tokyo/Japan</p>
        <h4>Email</h4>
          <p class="profile-text-description">catjp@protonmail.ch</p>
        <h4>Jobs</h4>
          <p class="profile-text-description">Frontend Engineer</p>
        <h4>Jobs History</h4>
          <p class="profile-text-description-history">4/1/2020-12/30/2020</p>
          <p class="profile-text-description">
            Programming learning service(Start up)<br>
            (HTML5,CSS3,JavaScript,Vue.js,Webpack,ESLint,Jest)
          </p>
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
          </p> -->
      </div>

      <p>The design was inspired by <a href="https://kristopolous.github.io/BOOTSTRA.386/index.html" target=”_blank”>BOOTSTRA.386</a></p>
    </div>
  </div>
</div>