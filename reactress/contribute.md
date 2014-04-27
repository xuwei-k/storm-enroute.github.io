---
layout: projdefault
projectname: Reactress
projectpath: reactress
logoname: reactress-mini-logo.png
title: Contributing
permalink: /contribute/index.html
---



### Source code

Please submit bug reports and feature requests at our [issue tracker at GitHub](https://github.com/storm-enroute/reactress/issues).
We'll be happy to take a look!

Feeling like contributing with some code?
Reactress source code is available at [GitHub](https://github.com/storm-enroute/reactress).
Simply fork us at GitHub and submit a pull request.
We will review it and merge your changes in.
Make sure to read the [contributor's guide](/dev/contribute/) first!


### License

Available [here](https://raw.githubusercontent.com/storm-enroute/reactress/master/LICENSE).

<span id="licensebox"></span>

<script>
var licensebox = document.getElementById("licensebox");
$.get("https://api.github.com/repos/storm-enroute/reactress/contents/LICENSE", function(data) {
  var icon = document.createElement('IMG');
  icon.setAttribute("src", "/resources/images/{{ page.logoname }}");
  icon.setAttribute("width", 32);
  var ltxt = window.atob(data.content);
  ltxt = ltxt.replace(/\t/g, '    ').replace(/  /g, '&nbsp; ').replace(/  /g, ' &nbsp;').replace(/\r\n|\n|\r/g, '<br />');
  licensebox.appendChild(icon);
  licensebox.innerHTML = licensebox.innerHTML + '<br/>' + ltxt;
});
</script>
