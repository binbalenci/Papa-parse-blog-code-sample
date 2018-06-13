```html
<!-- Using papa-parse with worker and stream -->
<papa-parse auto header worker stream script-path="../../papaparse/papaparse.min.js" fields="{{fields}}" url="https://some.domain/some.csv" on-stream="handleRecord"></papa-parse>

<script>
  function handleRecord(e, {data, meta, errors}) {
    console.log(data);
  }
</script>
```
