<h1><b>Explicações do funcionamento e regras sobre a folha de pagamentos:</b></h1>
  <h3>Regras:</h3>
    -O usuário deverá iniciar o sistema especificando o primeiro dia do ano (segunda, terça, quarta...) e inserindo a data atual como é pedido;<br>
    -O usuário deverá sempre inserir os dados da forma como o programa pede;<br>
    -Se o programa requisitar algum número decimal, ele deve ser digitado com o ponto (.) e com no máximo duas casas decimais, por exemplo o número 3.12;<br>
    -Caso o usuário deseje realizar alguma operação com algum funcionário, ele deverá ter pelo menos 1 funcionário registrado para realizar tal ação;<br>
    -O usuário deverá sempre inserir o dado requerido corretamente.<br>
    
  <h3>Funcionamento:</h3>
  -Ao pedir os dados iniciais sobre a data o programa irá calcular automaticamente os últimos dias de cada mês e os dias úteis de cada mês;<br>
  -Ao acionar a opção 0 o programa irá parar;<br>
  -Ao acionar a opção 1 o programa irá adicionar um novo empregado na matriz de empregados e irá calcular quantos dias faltam para o seu pagamento de acordo com o seu tipo de trabalho;<br>
  -Ao acionar a opção 2 o programa irá remover um empregado e moverá os empregados que estão em um índice maior do que o empregado que foi removido em uma posição para trás, ou seja, haverá um rearranjo na matriz;<br>
  -Ao acionar a opção 3 o programa irá pedir a hora e o minuto de entrada/saída e assim ele irá calcular a quantidade de horas que o funcionário trabalhou no dia que ele passou o cartão de ponto. Se o funcionário entrou no mesmo horário que ele saiu, o sistema pensará que o funcionário passou 24 horas trabalhando. Além disso o funcionário não pode passar mais de 24 horas trabalhando sem parar;<br>
  -Ao acionar a opção 4 o programa irá atribuir a venda naquela data para o funcionário especificado e irá acrescentar automaticamente ao seu salário o percentual que ele ganhou com a venda;<br>
  -Ao acionar a opção 5 o programa irá adicionar uma taxa de serviço ao funcionário especificado que será descontado do seu próximo contracheque;<br>
  -Ao acionar a opção 6 o programa fará uma série de escolhar para o usuário modificar algum dado do funcionário especificado ou não. Nessa opção, o programa implementado possui alguns detalhes que devem ser explicitados. Ao modificar o salário ou o tipo de trabalho, o contracheque do funcionário será reiniciado. Além disso, ao modificar o seu tipo de trabalho, haverá um reinício na quantidade de dias para o pagamento daquele funcionário de acordo com a agenda atual da empresa e a forma como é dada o pagamento para o seu tipo de trabalho, por exemplo, se um funcionário horista é modificado para um funcionário comissionado (assalariado com comissão), então a quantidade de dias para o pagamento será reiniciada e recalculada de acordo com a agenda bi-semanal da empresa. Um outro ponto importante é que se o funcionário pertence ao sindicato e sair, ele perderá apenas o id de sindicato e a taxa de sindicato automaticamente. Caso o funcionário entre em um sindicato, o usuário deverá escolher manualmente o seu id de sindicato e a taxa de sindicato;<br>
 -Ao acionar a opção 7 o usuário rodará a folha de pagamento avançando um dia. O programa identificará automaticamente quando deverá passar o mês, o ano e quando calcular um novo calendário. Durante a folha de pagamento, o sistema identifica se é o dia 1 (dia de pagamento da taxa de sindicato) e verifica quem é pago naquele dia, realizando o pagamento de acordo com os salários, as taxas a serem pagas e a forma como o pagamento deverá ser realizado. Ele sempre atualiza a quantidade de dias para o pagamento de todos os funcionários. Uma outra observação é que, se o funcionário não tiver um saldo positivo (ou neutro), ele não conseguirá pagar a taxa de serviço do sindicato e assim deverá esperar pelo próximo contracheque;<br>
 -Ao acionar a opção 8, o usuário poderá refazer(redo) e desfazer(undo) as suas ações. Toda vez que o usuário realiza uma ação (1, 2, 3, 4, 5, 6, 7, 9) a matriz de empregados é guardada na matriz de undo_redo
