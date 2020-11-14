<script>
</script>

<style>
.blinking{
  width: 4px;
  height: 4px;
  margin-left: 4px;
  background: #fff;
  -webkit-animation:blink .1s ease-in-out infinite alternate;
  -moz-animation:blink .1s ease-in-out infinite alternate;
  animation:blink 1.05s ease-in-out infinite alternate;
}
@keyframes blink{
  0% {opacity:0;}
  100% {opacity:1;}
}
</style>


<div class="blinking"></div>