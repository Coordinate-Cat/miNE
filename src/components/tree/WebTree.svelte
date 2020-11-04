<script>

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

const tree_info = [
  {title: 'Test', url: 'https://fontawesome.com/'},
];
tree_info.sort(compare);
</script>

<style>
h5::before {
  font-family: "Font Awesome 5 Free";
  content: '\f07c';
  font-size: 15px;
  margin-right: 5px;
  margin-left: 5px;
}
summary {
  cursor: pointer;
  outline: none;
  height: 20px;
}
summary::-webkit-details-marker {
  display: none;
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


<div class="tree">
  <ul>
    <li>
      <details open>
        <summary><h5>Web</h5></summary>
        <ul>

          <li>
            <details open>
            <summary><h5>Links</h5></summary>
            <ul>
              {#each tree_info as {title, url}}
              <li><a href="{url}">{title}</a></li>
              {/each}
            </ul>
            </details>
          </li>

        </ul>
      </details>
    </li>
  <!-- So far -->
  </ul>
</div>