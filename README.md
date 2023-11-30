# Micro-serviços em Java
Um projeto criado para entendimento de microserviços em java, sendo ele um composto por 2 microserviços. É um sistema de inscrições em eventos, na qual teremos uma lista de eventos disponíveis e a quantidade máxima de participantes. Ao se inscrever em um evento, o participante receberá um e-mail de confirmação de inscrição. <br/> 

**Observação:** Todo o conteúdo foi retirado da [live da Fernanda Kipper](https://youtu.be/yACzWg9gUGM)

## Micro-serviço de Evento
- Por retornar a lista de todos eventos disponíveis, filtrando pela data, retornando apenas aqueles que ainda não aconteceram;
- Por cadastrar novos eventos no banco de dados;
- Por receber as requisições de novas inscrições em um evento, salvando cada inscrição no banco de dados.
  
## Micro-serviço de Mensageria
Este serviço será responsável por: 
- Por disparar os e-mails. Recebendo as informações de cada email que deve ser enviado através do payload com remetente, body e assunto do e-mail.
Melhoria futura: consumir cada e-mail que deve ser enviado de uma fila, e os serviços que precisam enviar e-mail postam as informações nessa fila.
