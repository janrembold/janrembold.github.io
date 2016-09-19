##JS/CSS Build Blocks - Useref

* Automatisierter Buildprozess: Concat & Minify/Uglify
* Performance bei der Entwicklung

```javascript
<!-- build:js scripts/combined.js -->
<script type="text/javascript" src="scripts/one.js"></script>
<script type="text/javascript" src="scripts/two.js"></script>
<!-- endbuild -->
```