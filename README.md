
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="../css/style.css">
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
    <title>ALAYATL</title>
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
