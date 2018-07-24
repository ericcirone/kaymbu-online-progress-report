## Kaymbu Online Progress Report

Trouble viewing your Kaymbu Progress Report? Just copy the url from the failed page and then you will be able to view your child's progress report online.


<input type="text" id="url">
<button id="button">View Online Progress Report</button>

<script>
    var text = "";
    document.querySelector("#url").addEventListener("input", function (evt) {
        console.log(evt);
        text = evt.target.value;
    });
    document.querySelector("#button").addEventListener("click", function (evt) {
        console.log(text);

    });
</script>