# PHN-Task-1

HTML code:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style1.css">
    <title>Table Booking Form</title>
</head>
<body class="main_bg">
    <div class="form">
        <div class="form-text">
            <h1> .....Book Now.....</h1>
            <p>Book Your Table Now And Have A Great Meal!</p>
        </div>
        <div class="main-form">
            <form action="index.php" method="get">
                <div>
                    <span>Your full name ?</span>
                    <input type="text" name="name" id="name" placeholder="Write your name here..." required>
                </div>
                <div>
                    <span>Your email address ?</span>
                    <input type="email" name="name" id="name" placeholder="Write your email here..." required> 
                </div>
                <div>
                    <!-- <---this is the select option--->
                    <span>How many people ?</span>
                    <select name="people" id="people" required>
                        <option value=""><---People---></option>
                        <option value="1">1 People</option>
                        <option value="2">2 People</option>
                        <option value="3">3 People</option>
                        <option value="4">4 People</option>
                    </select>
                    <!-- <---this is the select option--->
                </div>
                <div>
                    <span>What time ?</span>
                    <input type="text" name="time" id="time" placeholder="Time" required>
                </div>
                <div>
                    <span>What is the date ?</span>
                    <input type="date" name="date" id="date" placeholder="date" required>
                </div>
                <div>
                    <span>Your phone number ?</span>
                    <input type="number" name="number" id="number" placeholder="Write your number here..." required>
                </div>
                <div id="submit">
                    <input type="submit" value="SUBMIT" id="submit">
                </div>
 </form>
        </div>
    </div>
</body>
</html>


CSS code:
@import url('https://fonts.googleapis.com/css2?family=Akaya+Telivigala&display=swap');
*{
    margin: 0;
    padding: 0;
}.main_bg{
    background-image: url(background3.jpg);
    max-width: 1280px;
    height: 800px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
}
.form{
    width: 650px;
}.form-text{
    text-align: center;
    margin: 0 0 40px 0;
}
.form-text h1 span img{
    margin: 0 10px;
}
.form-text h1{
    color: #fff;
    font-family: 'Akaya Telivigala', cursive;
    font-size: 40px;
    margin-bottom: 20px;
}
.form-text p{
    color: #fff;
    font-family: 'Akaya Telivigala', cursive;
    font-size: large;}
.main-form div{
    margin: 10px 10px;
    width: 300px;
    display: inline-block;
}
.main-form div input {
    width: 100%;
    font-family: 'Akaya Telivigala', cursive;
    background: none;
    border: 1px solid #ffca00;;
    font-size: 20px;
    color: #fff;
    outline: none;
    padding: 3px 0 3px 10px;
    margin-top: 10px;
}
.main-form div select{
    width: 104%;
    font-family: 'Akaya Telivigala', cursive;
    background: none;
    border: 1px solid #ffca00;;
    font-size: 20px;
    color: #fff;
    outline: none;
    padding: 3px 0 3px 10px;
    margin-top: 10px;
}
.main-form div span{
    width: 100%;
    font-family: 'Akaya Telivigala', cursive;
    color: #fff;
    font-size: 25px;
}

#submit{
    width: 100%;
    text-align: center;
}
#submit input{
    font-family: 'Akaya Telivigala', cursive;
    width: 200px;
    background-color: yellow !important;
    color: black !important;
    transition: all .3s;
}
#submit input:hover{
    font-family: 'Akaya Telivigala', cursive;
    width: 200px;
    background-color: black !important;
    color: #fff !important;
}
#submit input:active{
    font-size: 19px;
    background-color: rgb(46, 20, 5) !important;
    color: #fff !important;
}
@media screen and (max-width:710px) {
    .main-form{
        text-align: center;
    }
}
