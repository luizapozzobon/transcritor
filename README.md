# transcritor

Código para transcrever automaticamente clipes de áudio grandes em pt-br.
--------------
---- Instruções para primeira execução ----

1. Instalar Python
	1.1 Marcar a caixa da primeira tela do instalador de "Adicionar ao PATH" (ou algo assim)

2. Abrir o prompt do PowerShell ou cmd

	2.1 Digitar: pip install pydub
	
	2.2 Digitar: pip install ffpmeg-python
	
	2.3 Digitar: pip install SpeechRecognition

-------------

---- Instruções de uso ----

1. Abrir prompt do PowerShell ou cmd na pasta dos arquivos speech_to_text e transcritor

	(Shift + botão direito na pasta em que estão os arquivos de áudio e os códigos)

2. Digitar:

	python transcritor.py nome_do_arquivo.wav nome_do_arquivo2.wav


	- OBSERVAÇÕES:
	
	2.1 Pode botar quantos arquivos quiser para transcrever, mas sugiro não botar muitos se não demora muito tempo.
	
	2.2 O tempo de duração padrão para cada arquivo gerado é de 30 segundos, 
	se quiser alterar, executar o comando com o parâmetro "--duration=xx segundos".
	No exemplo abaixo, os áudios serão particionados em 40 segundos cada.

		python transcritor.py nome_do_arquivo.wav --duration=40

3. Aguardar. Os áudios serão particionados e transcritos automaticamente. 
Esses arquivos se encontrarão na pasta de nome igual ao arquivo de áudio principal.
