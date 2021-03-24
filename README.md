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
