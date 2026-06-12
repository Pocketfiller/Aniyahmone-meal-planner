<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Aniyahmone Meal Planner</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Literata:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

/* RESET */
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:linear-gradient(135deg,#fff9fb,#fff0f6,#fef6ff);
min-height:100vh;
color:#444;
}

/* MENU BUTTON */
.menu-btn{
position:fixed;
top:10px;
left:10px;
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

/* MENU */
.dropdown-menu{
position:fixed;
top:0;
left:-320px;
width:280px;
height:100%;
background:#ffffff;
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
color:#ff5c8a;
margin-bottom:15px;
}

.dropdown-menu a,
.week-btn{
display:block;
width:100%;
padding:12px;
margin-bottom:10px;
background:#ffe6f0;
color:#ff3f86;
text-decoration:none;
font-weight:600;
border:none;
border-radius:12px;
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
background:#ffffff;
padding:25px;
border-radius:20px;
text-align:center;
box-shadow:0 5px 15px rgba(0,0,0,.05);
}

.hero h1{
font-size:2.6rem;
color:#ff4f8b;
text-transform:uppercase;
font-family:'Literata',serif;
}

/* WEEK */
.week-card{
margin-top:20px;
background:#ffffff;
padding:20px;
border-radius:20px;
box-shadow:0 5px 15px rgba(0,0,0,.05);
}

.week-title{
font-size:1.5rem;
color:#ff4f8b;
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
background:#ffe6f0;
padding:14px;
font-weight:700;
cursor:pointer;
}

.day-content{
padding:15px;
background:#fff;
border:1px solid #f3f3f3;
}

/* MEALS */
.meal{
background:#fff7fa;
padding:12px;
border-radius:12px;
margin-bottom:10px;
display:flex;
gap:10px;
align-items:flex-start;
transition:.2s;
}

.meal.completed{
opacity:0.5;
text-decoration:line-through;
}

.meal h3{
color:#ff4f8b;
margin-bottom:5px;
font-size:1rem;
}

.nutrition{
font-size:.9rem;
line-height:1.6;
color:#555;
}

/* CHECKBOX */
.meal input{
margin-top:5px;
transform:scale(1.2);
accent-color:#ff4f8b;
cursor:pointer;
}

/* CONGRATS */
.congrats{
background:#ffe0ec;
padding:20px;
border-radius:15px;
text-align:center;
color:#ff2f78;
}

/* MOBILE */
@media(max-width:768px){
.hero h1{
font-size:2rem;
}
}

</style>
</head>

<body>

<div class="menu-btn" onclick="toggleMenu()">☰</div>

<div id="menu" class="dropdown-menu">
<h2>💕 Meal Planner</h2>
<a href="#home" onclick="closeMenu()">🏠 Home</a>
<button class="week-btn" onclick="toggleWeeks()">📅 Weekly Plans</button>
<div id="weeks" style="display:none;">
<a href="#week1" onclick="closeMenu()">Week June 15</a>
</div>
</div>

<div class="main">

<section id="home" class="hero">
<h1>WELCOME ANIYAHMONE 💖</h1>
<p>Open the menu to view your weekly meal plans.</p>
</section>

<section id="week1" class="week-card">

<div class="week-title">📅 Week June 15th</div>

<!-- MONDAY -->
<details open>
<summary>Monday</summary>
<div class="day-content">

<div class="meal">
<input type="checkbox" onchange="toggleMeal(this)">
<div>
<h3>Breakfast</h3>
Egg whites, whole egg, oatmeal, blueberries
<div class="nutrition">315 cal | 25g protein</div>
</div>
</div>

<div class="meal">
<input type="checkbox" onchange="toggleMeal(this)">
<div>
<h3>Lunch</h3>
Chicken breast, jasmine rice, zucchini
<div class="nutrition">430 cal | 42g protein</div>
</div>
</div>

<div class="meal">
<input type="checkbox" onchange="toggleMeal(this)">
<div>
<h3>Dinner</h3>
Salmon, sweet potato, green beans
<div class="nutrition">510 cal | 36g protein</div>
</div>
</div>

</div>
</details>

<!-- TUESDAY -->
<details>
<summary>Tuesday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Turkey sausage, eggs, strawberries</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Pork tenderloin, rice, asparagus</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Shrimp, rice, peppers</div></div>

</div>
</details>

<!-- WEDNESDAY -->
<details>
<summary>Wednesday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Protein oats, eggs, pineapple</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Ground turkey, sweet potato, spinach</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Cod, rice, green beans</div></div>

</div>
</details>

<!-- THURSDAY -->
<details>
<summary>Thursday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Egg whites, turkey bacon, fruit</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Chicken, sweet potato, cucumbers</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Pork loin, rice, zucchini</div></div>

</div>
</details>

<!-- FRIDAY -->
<details>
<summary>Friday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Eggs, oats, strawberries</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Ground turkey, rice, green beans</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Salmon, sweet potato, spinach</div></div>

</div>
</details>

<!-- SATURDAY -->
<details>
<summary>Saturday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Turkey sausage, egg whites, pineapple</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Chicken, rice, asparagus</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Shrimp stir fry, rice, peppers</div></div>

</div>
</details>

<!-- SUNDAY -->
<details>
<summary>Sunday</summary>
<div class="day-content">

<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Breakfast</h3>Eggs, oats, blueberries</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Lunch</h3>Pork tenderloin, sweet potato</div></div>
<div class="meal"><input type="checkbox" onchange="toggleMeal(this)"><div><h3>Dinner</h3>Chicken, rice, spinach</div></div>

<br>

<div class="congrats">
<h2>🎉 YOU DID IT!!</h2>
<p>Great job completing your week 💖</p>
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

function closeMenu(){
document.getElementById("menu").classList.remove("active");
}

function toggleMeal(box){
let meal = box.closest(".meal");
if(box.checked){
meal.classList.add("completed");
}else{
meal.classList.remove("completed");
}
}

</script>

</body>
</html>
