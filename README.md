Modelagem de Dados – Sistema de E-commerce
Sobre

Projeto de modelagem de dados de um sistema de vendas online, desenvolvido com foco em regras de negócio e consistência estrutural.
O modelo contempla clientes, pedidos, produtos, fornecedores, estoque, pagamento e entrega.

Principais Refinamentos Aplicados:
Cliente PF / PJ (Exclusividade)

A conta pode ser Pessoa Física ou Pessoa Jurídica
Nunca pode possuir CPF e CNPJ ao mesmo tempo
Implementação com atributo tipo_cliente e regra de exclusividade
Garante integridade cadastral
Evita inconsistência de dados

Pagamento

Cliente pode cadastrar múltiplas formas de pagamento
Pedido utiliza uma forma específica no momento da compra
✔ Modelagem 1:N entre Cliente e Forma de Pagamento
✔ Vínculo correto entre Pedido e Pagamento

🚚 Entrega

Cada pedido gera uma entrega
Entrega possui:
Status
Código de rastreio
✔ Separação adequada entre Pedido e Entrega
✔ Preparado para controle logístico

🏗 Estrutura Técnica

Uso de relacionamentos N:N quando necessário
Controle de quantidade por estoque
Suporte a múltiplos fornecedores por produto
Modelagem normalizada

🎯 Objetivo

Aplicar conceitos de modelagem relacional com foco em:
Regras de negócio reais
Integridade
Escalabilidade

Autor:
Luiz Felipe Ferraresso de Oliveira Alves
