```html
<!-- Parse from URL. -->
<papa-parse auto url="MOCK_DATA.csv" rows="{{rows}}"></papa-parse>
```

```html
<!-- Parse from raw CSV string. -->
<papa-parse auto raw="[[SomeCsvString]]" rows="{{rows}}"></papa-parse>
```

```html
<!-- Parse from FileReader -->
<input id="selectfile" type="file"></input>
<papa-parse auto file="[[file]]" rows="{{rows}}"></papa-parse>

<script>
  this.$.selectfile
  .addEventListener('change', function(e) {
    this.file = e.target.files[0];
  });
</script>
```
