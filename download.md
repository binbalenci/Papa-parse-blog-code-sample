```html
<papa-unparse header json-array="[[rows]]"></papa-unparse>
<button onclick="javascript:download">Download</button>

<script>
  function download() {
    document.querySelector('papa-unparse').downloadCsv('somefile.csv');
  }
</script>
```
