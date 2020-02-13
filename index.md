<!DOCTYPE html>
<head>
  <script type="text/javascript">

    function findFirstNonRepeating(num) {
        var origNum = (num.toString()).split('');
        var arr = (num.toString()).split('').sort();
        if (arr[0] != arr[1]) {
            return arr[0];
        } else while (arr[1] == arr[0] || arr[1] == arr[2]) {
            console.log(arr);
            arr.shift();
            if (arr.length == 0) {
              return "Oops, no non-repeating numbers here!"
              break;
            }
        }
        return arr[1];

    }


  </script>
</head>



<body>

<h1 style="color:red;text-align:center;font-size:24pt;font-family:Tahoma;"><em style="color:purple;">(Lowest)</em> Non-Repeating Digit Checker!</h1>
<div id="formbox" style="margin:auto;text-align:center;">
<input type="text" style="text-align:center;" id="dangus" name="field" placeholder="Put a number here!">
<input type="submit" onclick="alert(findFirstNonRepeating(document.getElementById('dangus').value))">
</div>







</body>
