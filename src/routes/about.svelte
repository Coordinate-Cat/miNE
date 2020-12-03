<script>
import WebTree from '../components/tree/WebTree.svelte';

const urlInfo = [
  {url: 'Web', title: 'links',},
  // {title: 'Test', link: 'tests', url: 'https://fontawesome.com/', urlname: 'stawesome'},
  // {title: 'fuck', link: 'fuck', url: 'https://fontawesome.com/', urlname: 'Testawesome'},
];

function compare(a, b) {
  const idA = a.title.toLowerCase();
  const idB = b.title.toUpperCase();
  let comparison = 0;
  if (idA > idB) {
    comparison = 1;
  } else if (idA < idB) {
    comparison = -1;
  }
  return comparison;
}
urlInfo.sort(compare);
// tree_links.sort(compare);


const tree_1st_title = [
  {title: 'Web', title2: 'links',},
  {title: 'Test', title2: 'fuck',},
  // {title: 'Test', link: 'tests', url: 'https://fontawesome.com/', urlname: 'stawesome'},
  // {title: 'fuck', link: 'fuck', url: 'https://fontawesome.com/', urlname: 'Testawesome'},
];
tree_1st_title.sort(compare);
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
}
.container {
  display: flex;
  margin: 20px;
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
</div>