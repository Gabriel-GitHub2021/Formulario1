# Formulario1
Meu Primeiro Formulário
---------------------------------HTML--------------------------------------

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
<link rel="stylesheet" type="text/css" href="formulario.css" media="screen">
    <title>Formulário</title>
</head>
<body>

    <div>
        <h1 id="titulo">Formulário 1</h1>
        <p id="subtitulo">Complete com suas informações.</p>
        <br>
    </div>
    
    <form>
        <fieldset class="grupo">
            <div class="campo">
                <label for="nome"><strong>Nome</strong></label>
                <input type="text" name="nome" id="nome" required>
            </div>

            <div class="campo">
                <label for="sobrenome"><strong>Sobrenome</strong></label>
                <input type="text" name="sobrenome" id="sobrenome" required> 
            </div>
        </fieldset>

        <div class="campo">
            <label for="email"><strong>Email</strong></label>
            <input type="email" name="email" id="email" required>
        </div>
    
        <div class="campo">
            <label><strong>De qual lado da aplicação você desenvolve?</strong></label>
            <label>
                <input type="radio" name="devweb" value="frontend" checked>Front-end
            </label>
            <label>
                <input type="radio" name="devweb" value="backend"> Back-End 
            </label>
            <label>
                <input type="radio" name="devweb" value="fullstack"> Fullstack
            </label>
        </div>

        <div class="campo">
            <label for="senioridade"><strong>Senioridade</strong></label>
            <select id="senioridade">
                <option selected disabled value="">Selecione</option>
                <option>Junior</option>
                <option>Pleno</option>
                <option>Sênior</option>
            </select>
        </div>

        <fieldset class="grupo">
            <div id="check">
                <label><strong>Selecione as tecnologias que utiliza:</strong></label>
                <input type="checkbox" id="tecnologia1" name="tecnologia1" value="HTML">
                <label for="tecnologia1">HTML</label>
                <input type="checkbox" id="tecnologia2" name="tecnologia2" value="CSS">
                <label for="tecnologia2">CSS</label>
                <input type="checkbox" id="tecnologia3" name="tecnologia3" value="Javascript">
                <label for="tecnologia3">Javascript</label>
                <input type="checkbox" id="tecnologia4" name="tecnologia4" value="PHP">
                <label for="tecnologia4">PHP</label>
                <input type="checkbox" id="tecnologia5" name="tecnologia5" value="C#">
                <label for="tecnologia5">C#</label>
                <input type="checkbox" id="tecnologia6" name="tecnologia6" value="Python">
                <label for="tecnologia6">Python</label>
                <input type="checkbox" id="tecnologia7" name="tecnologia7" value="Java">
                <label for="tecnologia7">Java</label>
            </div>
        </fieldset>
            
        <div class="campo">
            <br>
            <label><strong>Conte um pouco a sua experiência:</strong></label>
            <textarea row="6" style="width: 26em" id="experiencia" name="experiencia"></textarea>
        </div>

        <button class="botao" type="submit">Concluído</button>

        </div>
    </form>
</body>
</html>

----------------------------------------------------CSS---------------------------------------------------------

*{
    margin: 0;
    padding: 0;
}

#titulo{
    font-family: sans-serif;
    color: #380061;
    margin-left: 7%;
}

#subtitulo{
    font-family: sans-serif;
    color: #380061;
    margin-left: 5%;
}

#fieldset {
    border: 0;
}

body{
    background-color: #f0f0ff;
    font-family: sans-serif;
    font-size: 1em;
    color: #59429d;
    margin-left: 36%;
    margin-top: 2%;
    justify-content: center;
}

input, select, textarea, button{
    border-radius: 5px;
}

.campo {
    margin-bottom: 1em;
}

.campo label{
    margin-bottom: 0.2em;
    color: #59429d;
    display: block;
}

fieldset.grupo .campo{
    float: left;
    margin-right: 1em;
}

.campo input[type="text"], .campo input[type="email"], .campo select, .campo textarea {
padding: 0.2em;
border: 1px solid #59429d;
box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
display: block;
}

.campo select option{
    padding-right: 1em;

}

.campo input :focus, .campo select :focus, .campo textarea :focus {
    background: #e0e0f8;
}

.botao {
    font: 1.2em;
    background: #59429d;
    border: 0;
    margin-bottom: 1em;
    color: #ffffff;
    padding: 0.2em 0.6em;
    box-shadow: 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow: 1px 1px 1px rgba(0,0,0,0.5);
    position: absolute;
    top: 90%;
    left: 50%;
    margin-right: -50%;
    transform: translate(-50%, 50%);
}

.botao.hover {
    background: #ccbbff;
    box-shadow: inset 2px 2px 2px rgba(0,0,0,0.2);
    text-shadow: none;
}

.botao, select {
    cursor: pointer;
}

#check {
    display: inline-block;
}
