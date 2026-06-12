<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Aniyahmone's Meal Planner</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

/* RESET */
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:linear-gradient(135deg,#fff8fb,#ffeef5);
min-height:100vh;
color:#444;
}

/* TOP MENU */
.menu-btn{
position:fixed;
top:15px;
left:15px;
width:55px;
height:55px;
background:#ff9bbd;
color:white;
font-size:28px;
display:flex;
align-items:center;
justify-content:center;
border-radius:15px;
cursor:pointer;
z-index:9999;
box-shadow:0 5px 15px rgba(0,0,0,.08);
}

.dropdown-menu{
position:fixed;
top:0;
left:-320px;
width:280px;
height:100%;
background:#fff;
padding:20px;
transition:.3s;
z-index:9998;
overflow-y:auto;
box-shadow:5px 0 20px rgba(0,0,0,.05);
}

.dropdown-menu.active{
left:0;
}

.dropdown-menu h2{
color:#ff6f9d;
margin-bottom:15px;
}

.dropdown-menu a,
.week-btn{
display:block;
width:100%;
padding:12px;
margin-bottom:10px;
background:#ffe0ec;
color:#ff4f8b;
text-decoration:none;
font-weight:600;
border:none;
border-radius:12px;
text-align:left;
cursor:pointer;
}

/* MAIN */
.main{
padding:80px 15px 40px;
max-width:900px;
margin:auto;
}

/* HERO */
.hero{
background:#fff;
padding:25px;
border-radius:20px;
text-align:center;
box-shadow:0 5px 15px rgba(0,0,0,.05);
}

.hero h1{
font-size:2rem;
color:#ff5c8a;
margin-bottom:10px;
}

.hero p{
font-size:1rem;
color:#666;
}

/* WEEK CARD */
.week-card{
margin-top:20px;
background:#fff;
padding:20px;
border-radius:20px;
box-shadow:0 5px 15px rgba(0,0,0,.05);
}

.week-title{
font-size:1.5rem;
color:#ff5c8a;
font-weight:700;
margin-bottom:15px;
}

/* ACCORDION */
details{
margin-bottom:12px;
border-radius:12px;
overflow:hidden;
}

summary{
background:#ffe0ec;
padding:14px;
font-weight:700;
cursor:pointer;
}

.day-content{
padding:15px;
background:#fff;
border:1px solid #f3f3f3;
}

.meal{
background:#fff7fa;
padding:12px;
border-radius:12px;
margin-bottom:10px;
}

.meal h3{
color:#ff5c8a;
margin-bottom:5px;
font-size:1rem;
}

.nutrition{
font-size:.9rem;
line-height:1.6;
color:#555;
}

/* SUNDAY CONGRATS */
.congrats{
background:#ffd6e6;
padding:20px;
border-radius:15px;
text-align:center;
color:#ff2f78;
}

.congrats h2{
font-size:1.8rem;
margin-bottom:10px;
}

/* MOBILE FIX */
@media(max-width:768px){
.hero h1{
font-size:1.5rem;
}
}

</style>
</head>

<body>

<!-- MENU -->
<div class="menu-btn" onclick="toggleMenu()">☰</div>

<div id="menu" class="dropdown-menu">
<h2>💕 Meal Planner</h2>

<a href="#home">🏠 Home</a>

<button class="week-btn" onclick="toggleWeeks()">
📅 Weekly Plans
</button>

<div id="weeks" style="display:none;">
<a href="#week1">Week June 15</a>
</div>
</div>

<!-- MAIN -->
<div class="main">

<!-- HOME -->
<section id="home" class="hero">
<h1>Welcome Aniyahmone 💖</h1>
<p>Press the menu to access your weekly meal schedule.</p>
<p>Stay consistent, stay hydrated, trust the process.</p>
</section>

<!-- WEEK -->
<section id="week1" class="week-card">

<div class="week-title">📅 Week June 15th</div>

<!-- MONDAY -->
<details open>
<summary>Monday</summary>
<div class="day-content">

<div class="meal">
<h3>Breakfast</h3>
Egg whites, whole egg, oatmeal, blueberries
<div class="nutrition">315 cal | 25g protein | 30g carbs | 9g fat | 220mg sodium</div>
</div>

<div class="meal">
<h3>Lunch</h3>
Chicken breast, jasmine rice, zucchini
<div class="nutrition">430 cal | 42g protein | 45g carbs | 6g fat</div>
</div>

<div class="meal">
<h3>Dinner</h3>
Salmon, sweet potato, green beans
<div class="nutrition">510 cal | 36g protein | 35g carbs | 20g fat</div>
</div>

</div>
</details>

<!-- TUESDAY -->
<details>
<summary>Tuesday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Turkey sausage, 2 eggs, strawberries<div class="nutrition">340 cal | 26g protein</div></div>

<div class="meal"><h3>Lunch</h3>Pork tenderloin, brown rice, asparagus<div class="nutrition">450 cal | 40g protein</div></div>

<div class="meal"><h3>Dinner</h3>Shrimp, jasmine rice, peppers<div class="nutrition">420 cal | 38g protein</div></div>

</div>
</details>

<!-- WEDNESDAY -->
<details>
<summary>Wednesday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Protein oats, eggs, pineapple<div class="nutrition">390 cal | 30g protein</div></div>

<div class="meal"><h3>Lunch</h3>Ground turkey, sweet potato, spinach<div class="nutrition">450 cal | 38g protein</div></div>

<div class="meal"><h3>Dinner</h3>Cod, rice, green beans<div class="nutrition">390 cal | 36g protein</div></div>

</div>
</details>

<!-- THURSDAY -->
<details>
<summary>Thursday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Egg whites, turkey bacon, fruit<div class="nutrition">320 cal | 28g protein</div></div>

<div class="meal"><h3>Lunch</h3>Chicken, sweet potato, cucumbers<div class="nutrition">430 cal | 42g protein</div></div>

<div class="meal"><h3>Dinner</h3>Pork loin, rice, zucchini<div class="nutrition">470 cal | 40g protein</div></div>

</div>
</details>

<!-- FRIDAY -->
<details>
<summary>Friday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Eggs, oats, strawberries<div class="nutrition">370 cal | 31g protein</div></div>

<div class="meal"><h3>Lunch</h3>Ground turkey, rice, green beans<div class="nutrition">450 cal | 40g protein</div></div>

<div class="meal"><h3>Dinner</h3>Salmon, sweet potato, spinach<div class="nutrition">500 cal | 36g protein</div></div>

</div>
</details>

<!-- SATURDAY -->
<details>
<summary>Saturday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Turkey sausage, egg whites, pineapple<div class="nutrition">330 cal | 29g protein</div></div>

<div class="meal"><h3>Lunch</h3>Chicken, rice, asparagus<div class="nutrition">440 cal | 42g protein</div></div>

<div class="meal"><h3>Dinner</h3>Shrimp stir fry, rice, peppers<div class="nutrition">430 cal | 38g protein</div></div>

</div>
</details>

<!-- SUNDAY -->
<details>
<summary>Sunday</summary>
<div class="day-content">

<div class="meal"><h3>Breakfast</h3>Eggs, oats, blueberries<div class="nutrition">320 cal | 20g protein</div></div>

<div class="meal"><h3>Lunch</h3>Pork tenderloin, sweet potato<div class="nutrition">470 cal | 40g protein</div></div>

<div class="meal"><h3>Dinner</h3>Chicken, rice, spinach<div class="nutrition">430 cal | 42g protein</div></div>

<br>

<div class="congrats">
<h2>🎉 YOU DID IT!!</h2>
<p>Great job completing your week 💖</p>
<p>Next week drops Sunday night.</p>
</div>

</div>
</details>

</section>

</div>

<script>
function toggleMenu(){
document.getElementById("menu").classList.toggle("active");
}

function toggleWeeks(){
let w = document.getElementById("weeks");
w.style.display = w.style.display === "block" ? "none" : "block";
}
</script>

</body>
</html>
