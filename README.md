# Projeto Final Compasso Uol
**INTEGRANTES**:
 * Felipe Fernandes Gomes
 * Jhonatan Farias de lima
 * Kevin Collinys Silva Walke
 
---
## FUNCIONALIDADE: 

GET : /tempo/findPredictTimeWeek (Sem paramentro)
 * Realiza a busca dos dados no mock e convertem eles para portgues.
 * Realiza a conversao dos dados tratados para csv e grava o arquivo na maquina(Alterar o lugar de salvamento do arquivo em global.xml dentro do File config)
 * Realiza o envio do arquivo csv para um servidor FTP
 
GET : /tempo/findPredictTimeWeek (Com paramentro)
  * QueryParam = clima ("Chuva"): realiza a busca por um clima especifico, retornando os dados como dia, dia da semana,minima e maxima do respectivo dia que houver o clima igual a do paramentro.
  * QueryParam = semana(Ex: "Seg"): realiza a busca por dia da semana, retornando os dados como dia, dia da semana, minima e maxima do respectivo dia da semana que houver o dia da semana igual a do paramentro.
  * QueryParam = dia("28/07"): realiza a busca por data, retornando os dados como dia, dia da semana, minima e maxima do respectivo dia que houver a data igual a do paramentro.
  * OBS: Podemos passar qualquer tipo de paramentros para filtragem, alem de poder combinalos.
 
GET : /tempo/findPredictTimeWeek/media 
  * Realiza a media das temperaturas das pervisoes retornando dados como a media, dia ,dia da semana.
  
