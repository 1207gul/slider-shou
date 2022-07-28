# slider-shou

html>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Animation</title>

</head>
<body>
    <div class="slider">
        <figure>
            <div class="slide">
                <img src="./image/1.png" alt="img">
                <h1>manzara</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et ratione, omnis eaque quod quasi velit quia nobis quam qui magnam amet blanditiis aliquid, officiis nam vero repellendus explicabo hic veniam!</p>
            </div>
            <div class="slide">
                <img src="./image/2.png" alt="img">
                <h1>manzara</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et ratione, omnis eaque quod quasi velit quia nobis quam qui magnam amet blanditiis aliquid, officiis nam vero repellendus explicabo hic veniam!</p>
            </div>
            <div class="slide">
                <img src="./image/3.png" alt="img">
                <h1>manzara</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et ratione, omnis eaque quod quasi velit quia nobis quam qui magnam amet blanditiis aliquid, officiis nam vero repellendus explicabo hic veniam!</p>
            </div>
            <div class="slide">
                <img src="./image/4.png" alt="img">
                <h1>manzara</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et ratione, omnis eaque quod quasi velit quia nobis quam qui magnam amet blanditiis aliquid, officiis nam vero repellendus explicabo hic veniam!</p>
            </div>
        </figure>
    </div>
</body>
</html>

css>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

*{
    margin: 0;
    padding: 0;
}
@keyframes imageSlide{
    0%{
        left: 0;
    }
    10%{
        left: 0;
    }
    20%{
        left: -100%;
    }
    30%{
        left: -100%;
    }
    40%{
        left: -200%;
    }
    50%{
        left: -200%;
    }
    55%{
        left: -300%;
    }
    65%{
        left: -300%;
    }
    66%{
        left: -200%;
    }
    74%{
        left: -200%;
    } 
    75%{
        left: -100%;
    }
    85%{
        left: -100%;
    }
    90%{
        left: 0;
    }
    100%{
        left: 0;
    }
}

body{
    overflow-y: hidden;
}
/* .box{
    width: 100px;
    height: 100px;
    position: relative;
    background-color: red;
    left: 0;
    animation-name: transformation;
    animation-duration: 1s;
    animation-delay: 2s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
    animation-timing-function: cubic-bezier(1,-0.19, 0.57, 1.56);
    animation: 3s  transformation infinite alternate 2s;
} */

figure{
    position: relative;
    left: 0;
    width: 400%;
    display: flex;
    animation: 15s imageSlide infinite;
}
.slider{
    width: 100%;
    height: 100vh;
    background: #ccc;
    display: flex;
}

.slide{
    width: 1950px;
    position: relative;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.slide>img{
    width: 100%;
    height: 100vh;
}
.slide>h1{
    position: absolute;
    top: 450px;
}
.slide>p{
    position: absolute;
    top: 480px;
}
