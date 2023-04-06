### Itens feitos

<?php

$array = [
	
		1,
		'Maria',
		20,
		'Rua Marialva',
		'maria@email.com'

];

// cria arquivo 'w' -> Aberto apenas para escrita
$arquivo = fopen('file.csv', 'w'); 


//lista todas as informações do array
foreach($array as $users){
	fputcsv($arquivo, [$users], ';');
}


fclose($arquivo);

?>
