A minimalist framework based on my experience using JS frameworks.

# Usage

## Local file

```
<head>
  <script type="text/javascript" src="path/to/no.js"></script>
</head>
```

## Async external file

```
<script type="text/javascript">

(function() {
    var s = document.createElement('script');
    s.type = 'text/javascript';
    s.async = true;
    s.src = 'http://example.com/no.js';
    var x = document.getElementsByTagName('script')[0];
    x.parentNode.insertBefore(s, x);
})();

</script>
```
