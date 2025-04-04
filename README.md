# DESAFIO DE PROJETO DIO x HEINEKEN 🍺

## **Refinando um Projeto Conceitual de Banco de Dados  E-COMMERCE**



🎯 Este projeto tem como objetivo aplicar e refinar práticas de modelagem de banco de dados no contexto de um sistema de e-commerce.

---

## **Descrição do Projeto**
📚 Este projeto foi desenvolvido como parte do desafio do bootcamp **Heineken - Inteligência Artificial Aplicada a Dados com Copilot** e apresenta um modelo conceitual de banco de dados para um sistema de e-commerce. 

🎯 O objetivo é organizar eficientemente as informações relacionadas aos clientes, pedidos, pagamentos e entregas, garantindo escalabilidade e usabilidade.

---

## **Estrutura Conceitual e Refinamentos**

### **Clientes PJ e PF**
- 🧑‍💼 Cada cliente é identificado como **Pessoa Jurídica (PJ)** ou **Pessoa Física (PF)**, mas nunca ambos.
- **Implementação técnica:**
  - A tabela `Cliente` inclui o campo `Tipo_Cliente`, com valores restritos a "PJ" ou "PF".
  - ⚙️ Validação para garantir que um cliente tenha apenas informações de CPF ou CNPJ, de acordo com o tipo selecionado.

---

### **Pagamento**
- 💳 Clientes podem registrar múltiplas formas de pagamento.
- **Implementação técnica:**
  - Criação da tabela `Pagamento`, relacionada à tabela `Cliente` por meio da chave estrangeira `ID_Cliente`.
  - 📂 A tabela inclui os campos `Tipo_Pagamento` (ex.: cartão, boleto, Pix) e `Detalhes_Pagamento` para armazenar informações específicas.

---

### **Entrega**
- 🚚 Cada pedido possui status de entrega e um código de rastreio.
- **Implementação técnica:**
  - Criação da tabela `Entrega`, relacionada à tabela `Pedido` por meio da chave estrangeira `ID_Pedido`.
  - 🔍 A tabela inclui os campos `Status` (ex.: pendente, enviado, entregue) e `Codigo_Rastreio` para identificar a entrega.

---

## **Estrutura Proposta do Esquema**

| **Entidade**  | **Atributos**                                                                            |
|---------------|------------------------------------------------------------------------------------------|
| **Cliente**   | ID, Nome, Tipo_Cliente (PJ ou PF), CPF/CNPJ                                              |
| **Pedido**    | ID, ID_Cliente, Data, Total                                                             |
| **Pagamento** | ID, ID_Cliente, Tipo_Pagamento, Detalhes_Pagamento                                       |
| **Entrega**   | ID, ID_Pedido, Status, Codigo_Rastreio                                                  |

---

## **Relações Entre as Entidades**
- 🔗 **Cliente ↔ Pedido**: Um cliente pode realizar vários pedidos, mas cada pedido pertence a um único cliente.
- 💳 **Cliente ↔ Pagamento**: Um cliente pode cadastrar diversas formas de pagamento.
- 📦 **Pedido ↔ Entrega**: Cada pedido tem informações de entrega exclusivas.

---


## **Agradecimentos**
🎉 Agradeço à equipe da **DIO** e **HEINEKEN** pela oportunidade de realizar este desafio. Refinar o projeto conceitual de banco de dados foi fundamental para aprimorar minhas habilidades em modelagem e organização de dados.  
Este projeto reflete minha dedicação em seguir boas práticas e contribuir para um design eficiente e estruturado.

---

## Contato

Para dúvidas ou sugestões, entre em contato:
- **E-mail:** (sguimaraes1004@gmail.com)
- **Redes Sociais:** (https://www.linkedin.com/in/silvia-maria-guimar%C3%A3es-costa-3a01b423b)

---

🍺 _A parceria com a Heineken reforça o compromisso de promover a inovação e o aprendizado na área de tecnologia._

---


# ![DIO Logo](https://hermes.digitalinnovation.one/assets/diome/logo.png)
