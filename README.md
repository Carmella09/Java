# Java

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8" />
        <title></title>
    </head>
    <body>
        <script>
            alert("message");
            alert("Hello");

            var name = "Hello";
            document.write(name)
        </script>
    </body>
    </html>

------------------------------------------------

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8" />
        <title></title>
    </head>
    <body>
        <h1>Hello</h1>
        <p id="A"></p>

        <script>
            document.getElementById("A").innerHTML = 5 + 6;
        </script>

        <h1>Hello, my name is <span id="name"></span></h1>
        <script>
            let name = "Mella";
            document.getElementById("name").innerHTML = name;
        </script>

    </body>
    </html>

------------------------------------------------

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8" />
        <title></title>
        <style>
            img {
                display:none;
                width:100%;
            }
        </style>
    </head>
    <body>
        <div>
            <img src="https://picsum.photos/1000/301" />
            <img src="https://picsum.photos/1000/302" />
            <img src="https://picsum.photos/1000/303" />
        </div>
        <script>
            const images = document.querySelectorAll("img");
            let i = 0;
            setInterval(function () {

                if (i == 0) {
                    images[i].style.display = 'block';
                } else if (i == images.lenght) {
                    images[i - 1].style.display = 'none';
                    images[0].style.display = 'block';
                    i = 0;
                } else {
                    images[i - 1].style.display = 'none';
                    images[i].style.display = 'block';
                }i++;
            }, 2000);
        </script>

    </body>
    </html>




















