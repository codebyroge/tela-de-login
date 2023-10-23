<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login de adoção</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="main-login">
        <div class="left-login">
            <img src="cat-and-dog-animate.svg" class="laft-login-img" alt="Gato e cachorro animação">
        </div>
        <div class="right-login">
            <div class="card-login">
                <h1>LOGIN!</h1>
                <P>Não compre, adote!</P>
                <div class="textfield">
                    <label for="usuario">Usuário</label>
                    <input type="text" name="usuario" placeholder="Usuário"
                </div>
                <div class="textfield">
                    <label for="senha">Senha</label>
                    <input type="password" name="senha" placeholder="Senha"
                </div>
                <button class="btn-login">Login</button>
            </div>
        </div>
    </div>
</body>
</html>
CSS
@import url('https://fonts.googleapis.com/css2? family= Oswald:wght@500 & display=swap');
body{
    margin: 0;
    font-family: 'Oswald', sans-serif;
}
body * {
    box-sizing: border-box;
}
.main-login{
    width: 100vw;
    height: 100vh;
    background: #5cf64a;
    display:  flex;
    justify-content: center;
    align-items: center;
}

.left-login{
    width: 50vw;
    height: 100vh;
    display:  flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.left-login >h1{
    font-size: 3vw;
    color: aliceblue;
    font-weight: 900;
    margin: 0;
}
.left-login-img{
    width: 20vw;

}
.right-login{
    width: 50vw;
    height: 100vh;
    display:  flex;
    justify-content: center;
    align-items: center;
}
.card-login{
    width: 60%;
    display:  flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding: 30px 35px;
    background: #43b929;
    border-radius: 20px;
    box-shadow: 0px 10px 40px #00000056;
}
.card-login > h1 {
    color: #fbfffd;
    font-weight: 800;
    margin:  0;
}
.card-login >p {
    color: #fbfffd;
    font-weight: 800;
    margin:  0;
}
.textfield{
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    margin: 10px  0px;
}
.textfield > input{
    width: 100%;
    border: none;
    border-radius: 10px;
    padding: 15px;
    background: #ffffff;
    color: #000000de;
    font-size: 12pt;
    box-shadow: 0px 10px 40px #00000056;
    outline: none;
    box-sizing: border-box;
}

.textfield >label{
    color: #f0ffffde;
    margin-bottom: 10px;
}

.textfield > input::placeholder{
    color: #000000c9;
}

.btn-login{
    width: 80%;
    padding: 16px 0px;
    margin: 25px;
    border: none;
    border-radius: 80px;
    outline: none;
    text-transform: uppercase;
    font-weight: 800;
    letter-spacing: 3px;
    color: #2b134b;
    background: #5cf64a;
    cursor: pointer;
    box-shadow: 0px 10px 40px -12px #00ff8052;
}

@media only screen and (max-width: 600px){
    .main-login{
        flex-direction: column;

    }
    .left-login > h1 {
        display: none;
        height: auto;
    }
    .left-login{
        width: 80%;
        height: auto;
    }
    .right-login{
        width: 100%;
        height: auto;
    }
    .left-login-img{
        width: 30vh;
    }
    .card-login{
        width: 600%;
    }
}

