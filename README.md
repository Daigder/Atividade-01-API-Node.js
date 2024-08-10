# Atividade-01-API-Node.js

## Atividade proposta:

Fazendo requisições HTTP - Extra
Para encerrar este exercício, vamos adicionar uma validação no cep, para evitarmos enviar um cep inválido para a api que estamos consumindo.
Portanto, será necessário adicionar uma condição que faça um teste entre o cep informado na chamada a nossa api, e uma expressão regular (RegEx) que validará essas informações.
Em Javascript podemos criar uma expressão regular declarando uma variável/constante, passando o texto da expressão entre contra-barras ().
A expressão regular para validar cep é: 4[0-9]5}-?[09143}$
No Javascript ficará: const cepRegex = /^[0-9]{5}-?[09]{3}$/;
Para validar o cep informado contra a expressão regular usaremos cepRegex.test(cep), caso não seja válido deveremos retornar um status http 400 com a mensagem "CEP inválido. Formato:
XXXXX-XXX

### Imagem do Cep correto:

![Captura de tela Cep correto](https://github.com/user-attachments/assets/914ffabc-2b58-4c0b-98e7-b7289f36c6a1)

### Imagem do Cep incorreto:

![Captura de tela Cep incorreto](https://github.com/user-attachments/assets/9b3ee839-1ff6-45be-9a18-fe049137f721)

