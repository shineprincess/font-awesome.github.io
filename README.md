<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Advanced</title>
    <link href="https://fonts.googleapis.com/css2?family=Shadows+Into+Light&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

    <style type="text/css">

        *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Shadows Into Light', cursive;
            background: white;
        }

        :root {
            --width:100vw;
        }

        ::selection {
            background-color: chartreuse;
            color: cyan;
        }
        .main_div {
            width: 100vw;
            height: 100vh;
            text-align: center;
            padding-top: 100px;
            
        }

        h1 {
            color: lawngreen;
            font-size: 5rem;
        }


        h1::after {
            font-family: "Font Awesome 5 Free"; 
            content: "\f007";
            /* width: calc (var(--width) - 80vw) ; */
            width: 20vw;
            height: 25px;
            color: #1abc9c;
            font-size: 3rem;
            display: block;
            margin: 0 auto;
            border-bottom: 5px solid #3498;

        }

        @media(max-width: 768px) {
            h1{
                font-size: 4rem;
            }
            h1::after{
                height: 16px;
                font-size: 2rem;
            }
        }

        @media(max-width: 998px) {
            h1{
                font-size: 2.5rem;
            }
            h1::after{
                width: 30vw;
            }
        }
    </style>

</head>
<body>
    <div class="main_div">
        <h1>Shineprincess</h1>
    </div>
</body>
</html>
