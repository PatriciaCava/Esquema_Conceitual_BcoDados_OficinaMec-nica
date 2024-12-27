# Esquema_Conceitual_BcoDados_OficinaMecânica
Desafio Oficina Mecânica - DIO: Esquema do Projeto Conceitual do Banco de Dados

O projeto conceitual esquematizado para o desafio do 'sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica' possui as seguintes entidades e suas estruturas:

- Cliente: IdCliente, nome do cliente, documento, endereço, celular e e-mail.
- Carro: IdCarro, IdCliente associado, placa, modelo, fabricante, ano, cor, número do chassi e quilometragem.
- Mecânicos: IdMecânico, IdEquipe associado, nome do mecânico, endereço, celular, data de contratação, status, especialidade e certificações.
- Equipe: IdEquipe e Nome da equipe.
- Ordem de Serviço (OS): IdNúmeroOS, IdCarro associado, IdEquipe associado, data de emissão, valor total, status e data de conclusão.
- Mão de Obra: IdMãoDeObra, descrição e valor de referência dos serviços.
- Peças: IdPeças, Descrição e valor das peças.
- Pagamento: IdPagamento, IDOrdemDeServiços asociado, Valor total pago, método, status e data do pagamento.

e a definição dos relacionamentos 1:n são:

- Cliente - Carro
- Carro - Ordem Serviço
- Equipe - Mecânico
- Equioe - Ordem de serviço
- Ordem de serviço - pagamento
  
e dos relacionamentos n:n são:

- OS|MãoDeObra
- OS|Peça
  

