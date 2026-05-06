Clone o repositório primeiro e, em seguida, consulte o arquivo README para obter as instruções.

Projeto Sass - Aula Completa

Explicação
Este documento apresenta um exemplo completo de uso do Sass (SCSS), incluindo HTML, CSS e comandos de terminal.

Crie um arquivo com o nome index.html e copie o código HTML para dentro dele.

HTML (index.html)
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Projeto Sass</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<h1>Exemplo com Variáveis Sass</h1>
<p>Agora temos cores e tamanhos reutilizáveis</p>
<button>Clique aqui</button>
</body>
</html>


Crie uma pasta chamada SASS e, dentro dela, crie um arquivo chamado style.scss. Em seguida, cole o conteúdo do arquivo abaixo dentro dele.

SASS (style.scss)
$cor-fundo: #3498db;
$cor-texto: #ffffff;
$cor-botao: #2ecc71;
$tamanho-fonte: 18px;

body {
  background: $cor-fundo;
  font-family: Arial;
  text-align: center;
  padding: 50px;
  font-size: $tamanho-fonte;
}

h1 {
  color: $cor-texto;
  font-size: 32px;
}

p {
  color: $cor-texto;
}

button {
  background: $cor-botao;
  color: $cor-texto;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

Abra o terminal, seja pelo VS Code ou pelo terminal do computador, navegue até a pasta onde está o arquivo SASS utilizando o comando cd e, em seguida, execute o comando abaixo.

Comando no Terminal
sass --watch style.scss:style.css

Ao executar o comando, será gerado um arquivo style.css. Em seguida, faça a ligação desse arquivo no seu HTML.

Pronto, agora você poderá reutilizar as variáveis no seu projeto.