## Kaymbu Online Progress Report

Trouble viewing your Kaymbu Progress Report? Just copy the url from the failed page into the text box below and then you will be able to view your child's progress report online.


<input type="text" id="url" style="width: 100%; max-width: 800px;">
<button id="button">View Online Progress Report</button>

<p id="error" style="display:none;">Sorry that url is invalid. Please try again</p>

<script>
    var text = "";
    document.querySelector("#url").addEventListener("input", function (evt) {
        console.log(evt);
        text = evt.target.value;
    });
    document.querySelector("#button").addEventListener("click", function (evt) {
        console.log(text);

        var match = decodeURIComponent(text).match(/url=(.*)\?print/);
        if (match) {
            window.open(match[1], '_blank');
            document.querySelector("#error").style.display = "none";
        } else {
            document.querySelector("#error").style.display = "block";
        }
    });
</script>

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-122808643-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-122808643-1');
</script>
