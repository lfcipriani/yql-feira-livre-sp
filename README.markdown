This is a Yahoo Query Language (YQL) Open Table for searching for Markets in Sao Paulo.

----

Busca por Feiras Livres em São Paulo, por dia da semana e zona da cidade.
* As zonas possíveis são: CENTRAL, NORTE, SUL, LESTE e OESTE.
* Os dias da semana possíveis são: DOMINGO, TERÇA, QUARTA, QUINTA, SEXTA, SÁBADO.
* Deixe o dia da semana em branco para pesquisar em todos os dias de uma vez só.

----

Search for Free Markets in São Paulo (Brazil), by day of the week and city zone.
* Possibles zones are: CENTRAL, NORTE, SUL, LESTE e OESTE.
* Possible days of the week are: DOMINGO, TERÇA, QUARTA, QUINTA, SEXTA, SÁBADO.
* Don't mention the day of the week for a full week search.

## Exemplos/Sample queries

	use "http://github.com/lfcipriani/yql-feira-livre-sp/raw/master/yql-feira-livre-sp.xml" as feiras;
	select * from feiras where zone = 'SUL' and dayOfTheWeek = 'DOMINGO'
	
or
	use "http://github.com/lfcipriani/yql-feira-livre-sp/raw/master/yql-feira-livre-sp.xml" as feiras;
	select * from feiras where zone = 'OESTE'
	
[Try this on YQL console]: (http://query.yahooapis.com/v1/public/yql?q=use%20%22http%3A%2F%2Fgithub.com%2Flfcipriani%2Fyql-feira-livre-sp%2Fraw%2Fmaster%2Fyql-feira-livre-sp.xml%22%20as%20feiras%3B%0Aselect%20*%20from%20feiras%20where%20zone%20%3D%20'SUL'%20and%20dayOfTheWeek%20%3D%20'DOMINGO'  "Go to YQL console")