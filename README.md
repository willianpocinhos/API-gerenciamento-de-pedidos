<h1>API GERENCIAMENTO DE PEDIDOS</h1>
<h2>Funcionamento</h2>
<p>Foi desenvolvido um CRUD, para que fosse possível fazer a criação, leitura, atualização e exclusão dos pedidos.</p>

<h3>Método POST - Create Order</h3>
<p>Faz a criação do pedido.
  <br>
  Aqui é necessário preencher as seguintes informações: order, customer e value. O valor do ID é definido automaticamente, e após o pedido ser criado, o mesmo recebe o status 'Being prepared...', e uma mensagem é exibida: 'The order has been created!'.</p>
<br>
<h3>Método GET - Read Order List</h3>
<p>Faz a leitura de todos os pedidos existentes.
  <br>
  Ao fazer a chamada deste método, todos os pedidos existentes são exibidos, mostrando ID, order, customer, value e status. Caso não existam pedidos, uma mensagem é exibida: 'No order to show.'</p>
<br>
<br>
<p>Tecnologias utilizadas: Node.js, Express, Nodemon, uuid</p>


