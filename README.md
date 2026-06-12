# Aniyahmone-meal-planner
Aniyah’s Meal Plan Website 
<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">



<title>Aniyahmone's Meal Planner</title>



<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">



<style>



*{

margin:0;

padding:0;

box-sizing:border-box;

font-family:'Poppins',sans-serif;

}



body{

background:linear-gradient(135deg,#fff5f7,#ffe4ec);

min-height:100vh;

overflow-x:hidden;

}



/* Floating Background Graphics */



.floating{

position:fixed;

font-size:50px;

opacity:.12;

animation:float 8s ease-in-out infinite;

pointer-events:none;

}



.f1{top:10%;left:5%;}

.f2{top:20%;right:8%;}

.f3{bottom:15%;left:8%;}

.f4{bottom:10%;right:10%;}

.f5{top:55%;right:5%;}



@keyframes float{

50%{

transform:translateY(-20px);

}

}



/* Sidebar */



.sidebar{

position:fixed;

left:0;

top:0;

width:270px;

height:100%;

background:#ff9fbd;

padding:30px 0;

box-shadow:4px 0 20px rgba(0,0,0,.08);

overflow-y:auto;

}



.logo{

text-align:center;

font-size:26px;

font-weight:700;

color:white;

margin-bottom:30px;

}



.sidebar a{

display:block;

padding:16px 30px;

text-decoration:none;

color:white;

font-weight:600;

transition:.3s;

}



.sidebar a:hover{

background:#ff7ea6;

}



/* Main */



.main{

margin-left:270px;

padding:40px;

}



.hero{

background:white;

padding:50px;

border-radius:25px;

box-shadow:0 5px 20px rgba(0,0,0,.08);

text-align:center;

margin-bottom:30px;

}



.hero h1{

font-size:3rem;

color:#ff5c8a;

margin-bottom:15px;

}



.hero p{

font-size:1.15rem;

color:#666;

}



/* Week Section */



.week-card{

background:white;

padding:30px;

border-radius:25px;

box-shadow:0 5px 20px rgba(0,0,0,.08);

}



.week-title{

font-size:2rem;

font-weight:700;

color:#ff5c8a;

margin-bottom:20px;

}



/* Accordion */



details{

margin-bottom:15px;

border-radius:15px;

overflow:hidden;

}



summary{

background:#ffd6e3;

padding:18px;

cursor:pointer;

font-size:1.15rem;

font-weight:700;

}



.day-content{

padding:20px;

background:white;

border:1px solid #eee;

}



.meal{

background:#fff7fa;

padding:15px;

border-radius:15px;

margin-bottom:15px;

}



.meal h3{

color:#ff5c8a;

margin-bottom:10px;

}



.nutrition{

margin-top:10px;

line-height:1.8;

}



/* Congratulations */



.congrats{

background:linear-gradient(135deg,#ff6f9d,#ffb3c7);

padding:40px;

border-radius:20px;

text-align:center;

color:white;

animation:pulse 2s infinite;

margin-top:20px;

}



@keyframes pulse{

50%{

transform:scale(1.03);

}

}



.congrats h2{

font-size:2.5rem;

margin-bottom:10px;

}



/* Mobile */



@media(max-width:768px){



.sidebar{

position:relative;

width:100%;

height:auto;

}



.main{

margin-left:0;

padding:20px;

}



.hero h1{

font-size:2rem;

}



}



</style>

</head>

<body>



<div class="floating f1">🌹</div>

<div class="floating f2">🥤</div>

<div class="floating f3">🌸</div>

<div class="floating f4">🌹</div>

<div class="floating f5">🥤</div>



<div class="sidebar">



<div class="logo">

💕 Meal Planner

</div>



<a href="#home">🏠 Home</a>

<a href="#week1">📅 Week June 15th</a>



</div>



<div class="main">



<section id="home" class="hero">



<h1>Welcome Aniyahmone 💖</h1>



<p>

Press The Menu To Access Your Weekly Meal Prep Schedule.

</p>



<br>



<p>

Your new meal prep schedule will be added every week.

Stay consistent, stay hydrated, and trust the process.

</p>



</section>



<section id="week1" class="week-card">



<div class="week-title">

📅 Week June 15th

</div>



<details>

<summary>Monday</summary>



<div class="day-content">



<div class="meal">

<h3>🍳 Breakfast</h3>

3 Egg Whites, 1 Whole Egg, Oatmeal, Blueberries



<div class="nutrition">

Calories: 315<br>

Protein: 25g<br>

Carbs: 30g<br>

Fat: 9g<br>

Fiber: 5g<br>

Sodium: 220mg

</div>

</div>



<div class="meal">

<h3>🥗 Lunch</h3>

Grilled Chicken Breast, Jasmine Rice, Roasted Zucchini



<div class="nutrition">

Calories: 430<br>

Protein: 42g<br>

Carbs: 45g<br>

Fat: 6g<br>

Sodium: 130mg

</div>

</div>



<div class="meal">

<h3>🍽 Dinner</h3>

Salmon, Sweet Potato, Green Beans



<div class="nutrition">

Calories: 510<br>

Protein: 36g<br>

Carbs: 35g<br>

Fat: 20g<br>

Sodium: 120mg

</div>

</div>



</div>

</details>



<details>

<summary>Tuesday</summary>

<div class="day-content">

Copy Tuesday's meal plan here.

</div>

</details>



<details>

<summary>Wednesday</summary>

<div class="day-content">

Copy Wednesday's meal plan here.

</div>

</details>



<details>

<summary>Thursday</summary>

<div class="day-content">

Copy Thursday's meal plan here.

</div>

</details>



<details>

<summary>Friday</summary>

<div class="day-content">

Copy Friday's meal plan here.

</div>

</details>



<details>

<summary>Saturday</summary>

<div class="day-content">

Copy Saturday's meal plan here.

</div>

</details>



<details>

<summary>Sunday</summary>



<div class="day-content">



<div class="congrats">



<h2>🎉 YOU DID IT!! 🎉</h2>



<h3>Congratulations Aniyahmone 💖</h3>



<br>



<p>

You successfully completed your 7-Day Meal Prep Plan!

</p>



<br>



<p>

Next Week's Meal Plan Will Be Added On Sunday Night After Weekly Installment Fee.

</p>



<br>



<p>

🌹 Stay Consistent<br>

🥤 Stay Hydrated<br>

💪 Keep Building Muscle

</p>



</div>



</div>



</details>



</section>



</div>



</body>

</html>
