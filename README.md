# time-compact

Considere o armazenamento de um horário de forma compactada em uma única variável do tipo unsigened int (32 bits) onde:  os primeiros 14 bits permanecem zerados; os 6 bits seguintes são usados para armazenar a hora, os próximos 6 bits são utilizados para armazenar os minutos; e os últimos 6 bits são usados para armazenar os segundos. Por exemplo, considerando que tenhamos o seguinte horário: /

>Hora: 13
Minuto: 45
Segundo: 30

A representação binária em uma variável do tipo unsigened int (32 bits) seria:
 

                                     Hora   Minuto  Segundo 
                    00000000000000  001101  101101  011110
                                     
Faça uma função que receba um horário neste formato e retorne um horário no mesmo formato, mas com o valor correspondente ao segundo seguinte. Por exemplo, para o exemplo acima a função deverá retornar: 
 

                                     Hora   Minuto  Segundo 
                    00000000000000  001101  101101  011111
 

OBS: para o horário 23:59:59, o horário correspondente ao segundo seguinte seria 00:00:00.
