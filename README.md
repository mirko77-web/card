<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="wrapper">
        <div class="container">
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
            <div class="card">
                <div class="card-header">
                    <img src="https://images.pexels.com/photos/2121799/pexels-photo-2121799.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="fox">
                </div>
                <div class="card-body">
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Tempora autem dolorem necessitatibus nulla deleniti eum.</p>
                </div>
            </div>
        </div>
    </div>
</body>
</html>


-----------------/*codice css*/----------------------
:root {
    --n-card: 3;
    --card-gap: 2%;
    --card-width: calc((100% / var(--n-card)) - var(--card-gap));
    --card-base-rotation: 2deg;
    --animation-timing: 0.25s;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background-color: #F4F5F6;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.wrapper {
    width: 100%;
    display: flex;
    justify-content: center;
}

.container {
    max-width: 1120px;
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    gap: var(--card-gap);
    column-count: 3;
    column-gap: 30px;
 
}

.card {
    width: var(--card-width);
    border-radius: 15px;
    background-color: white;
    margin: 20px 0;
    opacity: 1;
    transition: all ease-in-out var(--animation-timing);
   transition: transform 0.3s, opacity 0.3s;

}


.card .card-header img {
    width: 100%;
    height: auto;
    border-radius: 15px 15px 0 0;
    
}

.card .card-body p {
    padding: 20px;
    
}



.card:nth-child(2n + 2) {
    transform: rotate(5deg);
    -ms-zoom-animation: default;
    
  
}



.card-header {
    display: flex;
    width: 100%;
    height: 200px;
    overflow: hidden;
    position: relative;
   
}

.card-header:hover {
    transform: scale(1.2);



}
.card-container .card:hover {
z-index: 10;
opacity: 1;
transform: scale(1.1);
}

.container:hover .card:not(:hover) {
opacity: 0.5;
}
