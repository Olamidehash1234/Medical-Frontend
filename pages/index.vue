<template>
    <div class="container">
        <div class="body-container">
            <h3 class="logo">LIFE<span class="cycle-span">CYCLE.</span></h3>
            <ul class="nav">
                <li class="nav-text"><a href="#">About Us</a></li>
                <li class="nav-text"><a href="#">Services</a></li>
                <li class="nav-text"><a href="#">Features</a></li>
                <li class="nav-text"><a href="#">Blog</a></li>
            </ul>
            <button class="nav-button">Contact us</button>
        </div>

        <div class="hero">
            <h1 class="hero-text">Experience Premium Healthcare, <br><span class="hero-textspan">Quality Services You Can Rely On</span></h1>
            <h2 class="hero-text2">Experience exceptional healthcare tailored to your needs. Trust Lifecycle for <br>compassionate, quality services that prioritize your wellbeing.</h2>
        </div>

        <div class="Container2">
            <img src="/static/surgery.jpg" alt="surgery image" class="image">
            <div class="overlay-form">
                <input type="text" placeholder="Name" class="input-field name-field" />
                <input type="datetime-local" placeholder="choose date and time" class="input-field datetime-field" />
                <select class="input-field select-field">
                <option>Cardiology</option>
                <option>Neurology</option>
                <option>Pediatrics</option>
                <option>Orthopedics</option>
                </select>
                <button class="book-now-button">Book Now</button>
            </div>
        </div>
    </div>

</template>


<script>

</script>


<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

.container{
    padding: 0;
    align-items: center;
    gap: 60px !important;
    box-shadow: 10px;
}

.body-container {
    justify-content: center;
    font-family: inter;
    display: flex;
    align-items: center;
    border: 2px;
    border-color: black; 
}

.logo{
    font-size: 30px;
    margin-right: 300px;
}

.nav{
    display: flex;
    text-decoration: none !important;
}
.nav-button{
    align-items: right;
    padding: 10px;
    border-radius: 9px;
    background-color: white;
    border-color: rgb(63, 125, 241);
    color: rgb(63, 125, 241);
    /* font-weight: 200px; */
    margin-left: 300px; 
    width: 8rem;
    cursor: pointer;
    font-size: 18px;
}

.nav-button:hover{
    background-color: rgb(63, 125, 241);
    color: white;
    transition: smooth;
}

ul{
    gap: 70px;
    list-style: none;
}
a{
    text-decoration: none;
    color:black;
}

.nav-text{
    font-size: 22px;
    font-style: normal;
}

.hero-text{
    text-align: center;
    font-size: 60px;
    font-family: poppins;
}

.hero-textspan{
    color: rgb(63, 125, 241);
}

.cycle-span{
    color: rgb(63, 125, 241);
    font-size: 34px;
}

.hero-text2{
    text-align: center;
}

.image{
    margin-top: 40px;
    justify-content: center !important;
    align-items: center !important;
    width: 1440px; 
    display: flex;
    margin-left: 70px; 
    border-radius: 30px;
    position: relative; /* Make it a positioning context for the overlay */
    
}

.container2 {
  width: 100%;
  text-align: center;
}

.overlay-form {
  position: absolute; /* Position the form relative to the container */
  bottom: -580px; /* Position it below the image */
  left: 50%; /* Center horizontally */
  transform: translateX(-50%); /* Adjust to exact center */
  display: flex;
  gap: 10px;
  background: white;
  padding: 10px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  z-index: 10; /* Ensure it appears above the image */
  width: 80%; /* Adjust width as needed */
  /* height: 50px; */
  padding-top: 30px;
  padding-left: 30px;
  padding-right: 30px;
  border: 0;
  font-family: inter;;
}

.input-field {
  padding: 10px;
  /* margin-top: 20px; */
  font-size: 16px;
  border: 1px solid #ddd;
  border-radius: 4px;
  /* height: 30px; */
  font-family: inter !important;
}

.name-field {
  flex: 2; /* Make the name input wider */
  font-family: inter !important;
}

.datetime-field,
.select-field {
  flex: 1; /* Make date/time and select inputs narrower */
}

.book-now-button {
  padding: 10px 20px;
  background-color: rgb(63, 125, 241);
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.book-now-button:hover {
  background-color: rgb(45, 85, 163);
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero-text {
    font-size: 40px;
  }

  .overlay-form {
    flex-direction: column;
    align-items: stretch;
    bottom: 0; /* Adjust positioning for smaller screens */
    transform: translateX(0); /* Adjust transform for centered alignment */
  }

  .input-field,
  .book-now-button {
    width: 100%;
    margin-bottom: 10px;
  }

  .book-now-button {
    margin-bottom: 0;
  }
}
</style>