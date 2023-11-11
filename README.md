# Current-TimeWebsite

http://127.0.0.1:5500/WebsiteTime.html

Developed Website Time
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Time</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <img src="Beach.jpg">
        <h1 id="Current-time"></h1>
        <div class="quotes">
        <p>TODAYS'QUOTE</p>
        <h2>Lost time is never found again.</h2>
        </div>
    </div>
    <script>
        let time = document.getElementById("Current-time");
        setInterval(()=>{
            let d = new Date();
        time.innerHTML = d.toLocaleTimeString();
        },1000)
        
    </script>
</body>
</html>

Style.CSS

*{
    margin: 0;
    padding: 0;
    font-family: "poppins, sans-serif";
    box-sizing: border-box;
}
.container{

    width: 100%;
    height: 100vh;
    background: #ffe3e3;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
}
.container img{
width: 100%;
}
.container h1{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    color: #fff;
    font-size: 90px;
    font-size: 600;
    letter-spacing: 3px;
}
.quotes{
    width: 100%;
    position: absolute;
    text-align: center;
    bottom: 15%;
    color: black;
    font-size: 20px;
    font-weight: 500;
}
.quotes h2{
    font-size: 45px;
    margin-top: 10px;
    font-weight: 500;
}

Bckground Image

