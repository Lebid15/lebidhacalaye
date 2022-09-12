
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="../css/style.css">
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
    <title>ALAYATL</title>
    <style>
        
* {
    margin: 0;
    padding: 0;
    text-decoration: none;
    box-sizing: border-box;
    list-style: none;
  }
  
  body {
    font-family: sans-serif;
  }

  nav {
    background: #00335a;
    height: 80px;
    width: 100%;
    letter-spacing: 3px;
  }

  label.logo {
    color: white;
    font-size: 35px;
    line-height: 80px;
    padding: 0 100px;
    font-weight: bold;
    letter-spacing: 3px;
  }

  nav ul {
    float: right;
    margin-right: 80px;
  }

  nav ul li {
    display: inline-block;
    line-height: 80px;
    margin: 0 5px;
  }

  nav ul li a {
    color: white;
    font-size: 25px;
    padding: 7px 13px;
    border-radius: 3px;
    text-transform: uppercase;
  }

  a.active,a:hover {
    background: #6d6d23;
    transition: .5s;
  }

  .checkbtn {
    font-size: 40px;
    color: white;
    float: right;
    line-height: 80px;
    margin-right: 50px;
    cursor: pointer;
    display: none;
  }

  #check {
    display: none;
  }

  @media (max-width: 952px) {
    label.logo {
        font-size: 30px;
        padding-left: 50px;
    }
    nav ul li a {
        font-size: 16px;
    }
  }

  @media (max-width: 858px) {
    .checkbtn {
        display: block;
    }
    ul {
        position: fixed;
        width: 100%;
        height: 100vh;
        background: #2c3e50;
        top: 80px;
        left: -100%;
        text-align: center;
        transition: all .5s;
    }
    nav ul li {
        display: block;
        margin: 50px 0;
        line-height: 30px;
    }
    nav ul li a {
        font-size: 20px;
    }
    a:hover,a.active {
        background: none;
        color: #0082e6;
    }
    #check:checked ~ ul {
        left: 0;
    }
  }

  section {
    background: linear-gradient(to right bottom, 
    #0245ff,
    #52ba62), url(img/5.jpg) no-repeat;
    background-size: cover;
    height: calc(100vh - 80px);
    color: white;
    padding: 40px 50px;
  }

  /*********************inputs****************************/
  .all-api {
    padding: 0px 10px;
  }

  .api {
    display: inline-block;
    margin: 20px 0px 20px 0;
    font-size: 20px;
  }

  .api input {
    width: 50%;
    padding: 4px 0px;
    font-size: 15px;
    font-weight: bold;
    text-align: center;
    letter-spacing: 2px;
  }

  
  @media (max-width: 858px) {
    .api input {
      font-size: 15px;
      width: 100%;
      padding: 5px 0;
      
    }
  }

  /*********************************************/
 
  .btn-design {
    margin-left: 20px;
    margin-top: 40px;
    width: 100%;
  }

  .btn {
    font-family: "roboto", sans-serif;
    font-size: 18px;
    font-weight: bold;
    background: #00ce8a;
    padding: 15px 70px;
    text-align: center;
    text-decoration: none;
    color: rgb(0, 0, 0);
    border-radius: 17px;
    cursor: pointer;
    border: none;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    transition: 0.3s;
  }
    /*, .btn:focus, .btn:active*/
  .btn:hover {
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
    background: #00ffaa;
    letter-spacing: 1px;
  }

  table {
    width: 100%;
    text-align: center;
    margin: 10px 0;
    font-family: 'Times New Roman', Times, serif;
  }

  th,td {
    padding: 5px;
  }

  #total {
    font-size: 19px;
    font-family: 'Times New Roman', Times, serif;
    letter-spacing: 3px;
    padding: 7px;
  }


  /**** table design ********/

  .table-title {
    text-align: center;
    font-size: 25px;
  }

  table {
    padding: 10px 0;
  }
  table tr {
    background-color: rgba(2, 2, 2, 0.507);
  }
  table tr th {
    background-color: rgba(9, 47, 68, 0.776);
    padding: 10px 0;
  }



  /********special designs*********/

  .totalo {
    background-color: rgb(131, 131, 0);
    border-bottom: rgb(0, 0, 0) solid ;
  }



    </style>
</head>
<body>
    <nav>
        <input type="checkbox" id="check">
        <label for="check" class="checkbtn">
            <i class="fa-light fa-bars"></i>
        </label>
        <label class="logo">ALAYATL</label>
        <ul>
            <li><a class="active" href="#">Home</a></li>
            <li><a href="#">Empty</a></li>
            <li><a href="#">Empty</a></li>
            <li><a href="#">Empty</a></li>
        </ul>
    </nav>

    <section>
        <div class="all-api">
            <div class="api">
                <label for="number-design" class="lebel-desing">Date</label>
                <input onkeyup="getTotal()" type="text" id="date">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Ruya</label>
                <input onkeyup="getTotal()" type="number" id="ruya">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Karma</label>
                <input onkeyup="getTotal()" type="number" id="karma">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Adil</label>
                <input onkeyup="getTotal()" type="number" id="adil">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Taim</label>
                <input onkeyup="getTotal()" type="number" id="taim">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Efix</label>
                <input onkeyup="getTotal()" type="number" id="efix">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Ashab</label>
                <input onkeyup="getTotal()" type="number" id="ashab">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Turkpin</label>
                <input onkeyup="getTotal()" type="number" id="turkpin">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Razer</label>
                <input onkeyup="getTotal()" type="number" id="razer">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Alfurat</label>
                <input onkeyup="getTotal()" type="number" id="alfurat">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Musaab</label>
                <input onkeyup="getTotal()" type="number" id="musaab">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Abu Talal</label>
                <input onkeyup="getTotal()" type="number" id="abutalal">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Kuvyet</label>
                <input onkeyup="getTotal()" type="number" id="kuvyet">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Ziraat</label>
                <input onkeyup="getTotal()" type="number" id="ziraat">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Codes</label>
                <input onkeyup="getTotal()" type="number" id="codes">
            </div>
            <div class="api">
                <label for="number-design" class="lebel-desing">Bayilar</label>
                <input onkeyup="getTotal()" type="number" id="bayilar">
            </div>

            <div>
                <small id="total"></small>
            </div>
        </div>

        <div class="btn-design">
            <button class="btn" id="submit">Calculate</button>
        </div>

        <div class="outputs">
            <p class="table-title">Daily Profit</p>
            <table>
                <tr>
                    <th>Date</th>
                    <th>Ruya</th>
                    <th>Karma</th>
                    <th>Adil</th>
                    <th>Taim</th>

                    <th>Efix</th>
                    <th>Ashab</th>
                    <th>Turkpin</th>
                    <th>Razer</th>
                    <th>Alfurat</th>
                    <th>Musaab</th>
                    <th>Abutalal</th>
                    <th>Kuvyet</th>
                    <th>Ziraat</th>
                    <th>Codes</th>
                    <th>Bayilar</th>

                    <th class="totalo">Total</th>
                    <th>Update</th>
                    <th>Delete</th>
                </tr>
            <tbody id="tbody">

                </tbody>
            </table>
        </div>

    </section>

    <script src="../js/main.js"></script>
</body>
</html>
