<head>
  <script type="text/javascript">
    function findFirstUnique(num) {
        var uniqArr = [];
        var total = 0;
        for (let i = 0; i < num.length; i += 1) {
          if ((num.split(num[total]).length -1) === 1) {
            uniqArr.push(num[total]);
          }
          total += 1;
        }
        if (uniqArr.length === 0) {
          return "Oops, no unique numbers here!"
        }
        return "First unique number: " + uniqArr[0];
    }

    function findAllUnique(num) {
        var uniqArr = [];
        var total = 0;
        for (let i = 0; i < num.length; i += 1) {
          if ((num.split(num[total]).length -1) === 1) {
            uniqArr.push(num[total]);
          }
          total += 1;
        }
        if (uniqArr.length === 0) {
          return "Oops, no unique numbers here!"
        }
        return "All unique numbers: " + uniqArr;
    }

  </script>
</head>
<body>
<h1 style="text-align:center;color:red;font-family:Verdana;">Unique Number: Redux</h1>
<div id="formbox" style="margin:auto;text-align:center;">
<input type="text" style="text-align:center;" id="dangus" name="field" placeholder="Put a number here!">
<input type="submit" value="First Unique Number" onclick="alert(findFirstUnique(document.getElementById('dangus').value))">
<input type="submit" value="All Unique Numbers" onclick="alert(findAllUnique(document.getElementById('dangus').value))">
</div>

</body>
