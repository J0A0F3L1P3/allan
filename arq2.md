* {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    user-select: none;
}

h1, h2, h3, h4, h5, h6{
    font-family: 'Gill Sans';
}

html,
body {
    width: 100%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: linear-gradient(144deg, #af40ff, #660099 50%, #00ddeb);
}

.desapareceClass {
    animation: desaparecendo 4s;
}

.apareceClass {
    animation: aparecer 2s;
}

.mov-section-esquerda {
    animation: mover-tela-esquerda 3s;
}

.mov-section-direita {
    animation: mover-tela-direita 3s;
}

.apt-section {
    background-color: #D3D3FF;
    height: 100%;
    width: 30%;
    min-width: 350px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border-radius: 0 15% 15% 0;
    padding: 0px 20px 0px 40px;
    gap: 2%;
    z-index: 3;
}
#password {
    margin: 0 0 0 0;
}
#username {
    margin: 0 0 15px 0;
}
.titulo {
    font-size: 41px;
}

.subtitulo {
    color: rgba(0, 0, 0, 0.578);
}

.section-form {
    display: none;
    background-color: #FFFFFF;
    width: min-content;
    height: min-content;
    flex-direction: column;
    align-items: center;
    padding: 30px;
    border-radius: 15px;
    animation: aparecer 1s;   
}
.nome-container {
    width: 100%;
    display: flex;
    gap: 2%;
    input {
        width: 100%;
    }
}
.messages {
    font-size: 12px;
    font-weight: 700;
    color: red; 
    letter-spacing: 0.8px;
    margin: 0 0 0 2px;
}
#cadastro-form {
    width: 100%;
}
.btn,
input {
    width: 320px;
    height: 17px;
    padding: 8px 10px 8px 10px;
    border-radius: 5px;
    border: 1px solid rgba(137, 46, 223, 0.518);
    margin: 12px 0 0 0;
}
input {
    margin: 15px 0 0 0;
    font-size: 13px;
}
input:focus {
    outline: 1px solid rgba(137, 46, 223, 0.941);
}
.btn {
    cursor: pointer;
    height: 36px;
    width: 100%;
    background-color: rgb(138, 46, 223);
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;
}
.text-content {
    width: 100%;
    display: flex;
    justify-content: space-between !important;
    margin: 2px;
    margin-bottom: 10px;
    
    h2 {
        font-size: 25px;
    }
    
    h3 {
        font-size: 15px;
    }

    .logo{
        width: 10%;
        height: 10%;
    }
}
#alert-content {
    font-weight: 700;
    color: red;
    font-size: 13px;
    width: 100%;
    padding: 3% 0px 0px 5%;
}
@keyframes aparecer {
    0% {
        opacity: 0%;
    }

    100% {
        opacity: 100%;
    }
} 
.formulario {
    position: absolute;
    left: 51%;
    background-color: #FFFFFF;
    width: min-content;
    /* max-width: 300px; */
    height: min-content;

    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 35px 30px 30px 30px;
    border-radius: 15px;
}

.text-content,
.esqueci-minha-senha-content {
    width: 100%;
    height: min-content;
    display: flex;
    justify-content: space-between;
}

.error {
    color: red;
    padding: 11px 2px 10px 2px;
    /*font-size: 14px; */
}

.esqueci-minha-senha-content {
    justify-content: space-between;

    span {
        margin: 12px 10px 10px 10px;
        font-size: 14px;
    }
}

#btn-cadastro{
    width: 49%;
}

#btn-login-scream{
    cursor: pointer;
    display: none;
    position: absolute;
    border-radius: 100%;
    top: 5%;
    left: 3%;
    width: 40px;
    height: 40px;
    background: linear-gradient(144deg, #af40ff, #660099 50%, #00ddeb);
    border: none;
    align-items: center;
    justify-content: center;
}
.imagem-voltar {
    width: 100%;
    height: auto;
}
.btn,
input {
    width: 320px;
    height: 17px;
    padding: 8px 10px 8px 10px;
    border-radius: 5px;
    border: 1px solid rgba(137, 46, 223, 0.518);
}

input {
    margin: 15px 0 0 0;
    font-size: 13px;
}

input:focus {
    outline: 1px solid rgba(137, 46, 223, 0.941);
}

.btn {
    height: 36px;
    width: 100%;
    /* border: 1.2px solid rgba(137, 46, 223, 0.518); */
    background-color: rgb(138, 46, 223);
    color: white;
    display: flex;
    align-items: center;
    justify-content: center;

}

.logo_login{
    width: 10%;
}

.btn:hover {
    outline: 1px solid rgba(137, 46, 223, 0.941);
    cursor: pointer;
}

.botton-content {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
    width: 100%;

    div {
        width: 100%;
    }
}

.button-content {
    display: flex;
    justify-content: space-between;
}

.span-content {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 30px;

    span {
        letter-spacing: 1.5px;
    }
}

.img-content {
    display: flex;
    justify-content: end;
    width: 10%;

    img {
        width: 100%;
        height: auto;
    }
}

.btncadastro {
    color: #609;
    text-decoration: none;
    font-size: 25px;
    border: none;
    background: none;
    font-weight: 600;
    font-family: 'Poppins', Gill Sans;
    cursor: pointer;
  }
  
  .btncadastro::before {
    margin-left: auto;
  }
  
  .btncadastro::after, .btncadastro::before {
    content: '';
    width: 0%;
    height: 4px;
    background: linear-gradient(144deg, #af40ff, #5b42f3 50%, #00ddeb);
    display: block;
    transition: 0.4s;
  }
  .btncadastro:hover::after, .btncadastro:hover::before {
    width: 100%;
  }

  @keyframes mover-tela-esquerda {
    0% {
        width: 30%;
        border-radius: 0 15% 15% 0;
    }

    100% {
        width: 100%;
        border-radius: 0 0 0 0;

    }
}

@keyframes mover-tela-direita {
    0% {
        width: 100%;
        border-radius: 0 0 0 0;
    }

    100% {
        width: 30%;
        border-radius: 0 15% 15% 0;
    }
}

@keyframes desaparecendo {
    0% {
        opacity: 100%;
    }

    50% {
        opacity: 0%;
    }

    100% {
        opacity: 0%;
    }
}

@keyframes aparecer {
    0% {
        opacity: 0%;
    }

    100% {
        opacity: 100%;
    }
}  
