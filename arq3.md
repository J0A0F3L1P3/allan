{% load static %}
<!DOCTYPE html>
<head>
    <link rel="stylesheet" href="{% static 'css/login.css' %}">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap" rel="stylesheet">
    <link rel="icon" type="image/x-icon" href="{% static 'images/logo-infra.png' %}">
    <title>Vivo InfraVision</title>
</head>
<body>
    <div class="formulario">
        <div class="text-content">
            <h1>Acesse o Portal</h1>
            <img class="logo_login" src="{% static 'images/vivo-119.png' %}" alt="">
        </div>
        <form method="post">
            {% csrf_token %}
            <label for="username">Usuário:</label>
            <input type="text" id="username" name="username" required>          
            <label for="password">Senha:</label>
            <input type="password" id="password" name="password" required>
            <div class="esqueci-minha-senha-content">
                <div class="error">
                    {% if error %}
                    <span> {{error}} <a href="" id="esqueci-minha-senha">Esqueci minha senha</a></span>
                    {% endif %}
                </div>
            </div>
            <div class="botton-content">
                <div class="button-content">
                    <button name="login" type="submit" class="btn" id="submit-login">Entrar</button>
                </div>    

            </div>    
        </form>
        <div class="span-content">    
            <button class="btncadastro" id="cadastrar">Cadastre-se</button>      
        </div>        
    </div>
    <section class="apt-section" id="apt-section">
        <button id="btn-login-scream">
            <img class="imagem-voltar" src="{% static 'images/seta-esquerda.png' %}" alt="">
        </button>
        <h1 id="titulo" class="titulo">Seja bem-vindo(a)</h1>
        <h3 class="subtitulo">Ger. Planejamento e Engenharia de Infraestrutura</h3>
        <section class="cadastro-section">
            <section class="section-form">
                <div class="text-content">
                    <div>
                        <h2>Cadastre-se</h2>
                        <h3>Dir. Engenharia de Infraestrutura e planejamento</h3>
                    </div>           
                    <img class="logo" src="{% static 'images/vivo-119.png' %}" alt="">
                </div>
                <form action="/cadastro/" method="post" id="cadastro-form">
                    {% csrf_token %}
                    <input type="text" placeholder="RE" id="reId" name="reId" required>
                    <label class="messages" for="reId">{{ re }}</label>
                    <input type="email" placeholder="E-mail" id="email" name="email" required>
                    <label class="messages" for="email">{{ email }}</label>
                    <input type="date" placeholder="Data de nascimento" id="data-nascimento" name="data_nascimento" disabled>
                    <div class="nome-container">
                        <input type="text" placeholder="Nome" id="nome" name="nome" required>
                        <input type="text" placeholder="Sobrenome" id="sobrenome" name ="sobrenome" required>
                    </div>
                    <input type="password" placeholder="Senha" id="senha-cadastro" name="password" required>
                    <input type="password" placeholder="Confirmar senha" id="confirmar-senha" name="confirmar_senha" required>
                </form>
                <ul id="alert-content"></ul>
                </div>
                <button class="btn" id="btn"></button>
            </section>
            <script src="index.js"></script>
        </section>
    </section>
    <script src="{% static 'js/screenLoginAnimation.js' %}"></script>
    <script src="{% static 'js/validaSenha.js' %}"></script>
</body>
</html> 
