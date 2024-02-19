<h1>API GERENCIAMENTO DE PEDIDOS</h1>
<h2>Funcionamento</h2>
<p>Foi desenvolvido um CRUD, para que fosse possível fazer a criação, leitura, atualização e exclusão dos pedidos.</p>

<h3>Método POST - Create Order</h3>
<p>Faz a criação do pedido.
  <br>
  Aqui é necessário preencher as seguintes informações através do body: order, customer e value. O valor do ID é definido automaticamente, e após o pedido ser criado, o mesmo recebe o status 'Being prepared...', e uma mensagem é exibida: 'The order has been created!'.</p>

<h3>Método GET 1 - Read Order List</h3>
<p>Faz a leitura de todos os pedidos existentes.
  <br>
  Ao fazer a chamada deste método, todos os pedidos existentes são exibidos, mostrando ID, order, customer, value e status. Caso não existam pedidos, uma mensagem é exibida: 'No order to show.'</p>

<h3>Método GET 2 - Read 1 Order</h3>
<p>Faz a leitura de apenas um pedido.
  <br>
  Aqui é necessário passar o ID do pedido através da URL. Antes do pedido ser exibido é feita a passagem por uma MIDDLEWARE (checkOrderId), com o objetivo de verificar a existência do ID. Caso o ID seja encontrado, o pedido é exibido, caso contrário, é exibida uma mensagem de erro: 'Order not found!'</p>

<h3>Método PUT - Update Order</h3>
<p>Faz a alteração de algum pedido.
  <br>
  Aqui é necessário passar o ID do pedido através da URL, e, fazer as alterações necessárias através do body. Antes do pedido ser exibido é feita a passagem por uma MIDDLEWARE (checkOrderId), com o objetivo de verificar a existência do ID. Caso o ID seja encontrado, o pedido é alterado, e as alterações são exibidas juntamente com uma mensagem: '>>> ORDER UPDATED <<<', caso contrário, é exibida uma mensagem de erro: 'Order not found!'</p>

<h3>Método DELETE - Delete Order</h3>
<p>Exclui algum pedido.
  <br>
  Aqui é necessário passar o ID do pedido através da URL. Antes do pedido ser excluído é feita a passagem por uma MIDDLEWARE (checkOrderId), com o objetivo de verificar a existência do ID. Caso o ID seja encontrado, o pedido é excluído e é exibida uma mensagem na tela: 'The order has been deleted!', caso contrário, é exibida uma mensagem de erro: 'Order not found!'</p>

<h3>Método PATCH - Order Ready</h3>
<p>Atualiza o status do pedido.
  <br>
  Aqui é necessário passar o ID do pedido através da URL. Antes do status ser atualizado é feita a passagem por uma MIDDLEWARE (checkOrderId), com o objetivo de verificar a existência do ID. Caso o ID seja encontrado, o status do pedido é atualizado, e todas as informações do pedido são exibidas juntamente com uma mensagem: '>>> THE ORDER IS READY <<<', caso contrário, é exibida uma mensagem de erro: 'Order not found!'</p>
  
<br>
<br>
<p>Tecnologias utilizadas: Node.js, Express, Nodemon, uuid</p>


