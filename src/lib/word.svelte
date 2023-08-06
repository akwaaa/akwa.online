<script>

var words = ['ākwa ↯', 'evee <3', 'eve/lou!!'],
    part,
    i = 0,
    offset = 0,
    len = words.length,
    forwards = true,
    skip_count = 0,
    skip_delay = 15,
    speed = 150;
var wordflick = function () {
  setInterval(function () {
    if (forwards) {
      if (offset >= words[i].length) {
        ++skip_count;
        if (skip_count == skip_delay) {
          forwards = false;
          skip_count = 0;
        }
      }
    }
    else {
      if (offset == 0) {
        forwards = true;
        i++;
        offset = 0;
        if (i >= len) {
          i = 0;
        }
      }
    }
    part = words[i].substr(0, offset);
    if (skip_count == 0) {
      if (forwards) {
        offset++;
      }
      else {
        offset--;
      }
    }
  },speed);
};

wordflick()

</script>

<h1>{part} | she/they | anarchist transfem catgirl Ⓐ</h1>

<style>

h1 {
  color: white;
  font-size: 30px;
  font-family: Inter;
  font-weight: 400;
  word-wrap: break-word;
  line-height: 1;
}

</style>