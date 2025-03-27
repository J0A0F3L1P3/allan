const secEsquerda = document.getElementById('apt-section')
const btnCadastrar = document.getElementById('cadastrar')
const formularioCadastro = document.querySelector('.section-form')
const titulo = document.querySelector('.titulo')
const subtitulo = document.querySelector('.subtitulo')
const formularioLogin = document.querySelector('.formulario')
const btnVoltar = document.getElementById('btn-login-scream')

btnCadastrar.addEventListener('click', ()=>{
    secEsquerda.classList.add('mov-section-esquerda')
    titulo.classList.add('desapareceClass')
    subtitulo.classList.add('desapareceClass')
    btnVoltar.classList.add('apareceClass')

    setTimeout(()=>{
        titulo.style.display = 'none'
        subtitulo.style.display = 'none'
        formularioLogin.style.display = 'none'
        document.querySelector('.cadastro-section').style.display = 'flex'
        formularioCadastro.style.display = 'flex'
        btnVoltar.style.display = 'flex'
    },2000)

    setTimeout(()=>{
        btnVoltar.classList.remove('apareceClass')
        titulo.classList.remove('desapareceClass')
        subtitulo.classList.remove('desapareceClass')
        secEsquerda.classList.remove('mov-section-esquerda')
        secEsquerda.style.width = '100%'
        secEsquerda.style.alignItems = 'center'
        secEsquerda.style.borderRadius = '0%'
    },2800)
})

document.getElementById('btn-login-scream').addEventListener('click', ()=>{
    const telaCadastro = document.querySelector('.cadastro-section')
    btnVoltar.classList.add('desapareceClass')
    telaCadastro.classList.add('desapareceClass')
    secEsquerda.classList.add('mov-section-direita') 
    titulo.classList.add('apareceClass')
    subtitulo.classList.add('apareceClass')
    formularioLogin.classList.add('apareceClass')

    setTimeout(()=>{
        btnVoltar.style.display = 'none'
        telaCadastro.style.display = 'none'
        titulo.style.display = 'block'
        subtitulo.style.display = 'block'
        document.querySelector('.formulario').style.display = 'flex'
    },1000)
    
    setTimeout(()=>{
        secEsquerda.style.width = '30%'
        secEsquerda.style.borderRadius = '0 15% 15% 0'
    }, 2000)

    setTimeout(()=>{
        telaCadastro.classList.remove('desapareceClass')
        secEsquerda.classList.remove('mov-section-direita') 
        titulo.classList.remove('apareceClass')
        subtitulo.classList.remove('apareceClass')
        formularioLogin.classList.remove('apareceClass')
        btnVoltar.classList.remove('desapareceClass')

    },3001)
})
 
