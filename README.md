by yahya
<html>
    <head>
        <style>
      .outer {
        margin: auto;
        height: 300px;
        width: 400px;
        border: 2px solid black;
        position: relative;
      }
      p {
        margin-left: 80px;
      }
      .in {
        margin-left: 80px;
        padding: 10px;
      }
      #bt {
        margin-top: 20px;
        position: absolute;
        left: 150px;
      }
      #bt:hover {
        background: green;
        font-size: 13px;
        cursor: pointer;
        color: white;
      }
    </style>
        <script>
      function fa() {
        if (a.value == "" || b.value == "") {
          f();
          document.getElementById("a").style.border = "3px solid red";
          document.getElementById("b").style.border = "3px solid red";
          bt.value = " u cant, bro ";
        } else {
          document.getElementById("a").style.border = "3px solid green";
          document.getElementById("b").style.border = "3px solid green";
          bt.value = "hanta ktbtihom";
          bt.style.left = "120px";
        }
      }
      flag = 1;
      function f() {
        if (flag == 1) {
          bt.style.left = "210px";
          flag = 2;
        } else if (flag == 2) {
          bt.style.left = "80px";
          flag = 1;
        }
      }
    </script>
    </head>
    <body>
        <div class="outer">
            <h1 style="text-align: center">Legend form</h1>
            <p>Entre your name</p>
            <input class="in" type="text" placeholder="Entre your name"
                id="a" />
            <p>Entre your password</p>
            <input
                class="in"
                type="password"
                placeholder="Entre your password"
                id="b" />
            <br />
            <input
                type="submit"
                onmouseenter="fa()"
                onclick="alert('one piece 3mk')"
                id="bt" />
        </div>
    </body>
</html>
