# Simulador de Quiz Interativo - André Gonçallez

Este é um simulador de quiz interativo em formato **HTML puro**, fácil de usar e personalizar. Ideal para estudos de nível intermediário e avançado em tecnologia, cibersegurança, redes, programação, e outras áreas técnicas.

---

## Sobre o Simulador

- Desenvolvido para rodar **offline** diretamente no navegador, sem necessidade de servidor.
- Layout simples, moderno e responsivo, com boa usabilidade em desktop e mobile.
- Permite escolher nível das perguntas: **Intermediário** ou **Avançado**.
- Permite configurar o número de questões e o tempo por questão.
- Feedback imediato após cada resposta, com explicação detalhada.
- Apresenta pontuação, acertos, erros e progresso.
- Possui timer individual por questão, com autoavaliação ao fim do tempo.

---

## Como usar

1. Abra o arquivo `Simulador_Quiz_Interativo_André.html` em qualquer navegador moderno (Chrome, Firefox, Edge, Safari).
2. Selecione o nível (Intermediário ou Avançado).
3. Defina o número de questões desejado (mínimo 5, máximo 100).
4. Configure o tempo para responder cada questão (em segundos).
5. Clique em **Iniciar Simulado** e comece a responder as perguntas.
6. Use o botão **Confirmar Resposta** para enviar sua resposta.
7. Veja a explicação da resposta e clique em **Próxima Questão** para avançar.
8. Ao final, será exibido seu desempenho geral.

---

## Como adicionar novas perguntas

No arquivo HTML, as perguntas ficam dentro da variável `QUESTIONS`, no bloco JavaScript.

Exemplo do formato das perguntas:

```js
{
  id: "identificador_unico",  // ex: "i4", "a15", "python01"
  level: "intermediate" ou "advanced",
  question: "Texto da pergunta",
  options: ["Opção 1", "Opção 2", "Opção 3", "Opção 4"],
  answer: índice da opção correta (começa em 0),
  explanation: "Texto com a explicação da resposta correta."
},
Exemplo real:
js
Copiar
Editar
{
  id: "i4",
  level: "intermediate",
  question: "Qual comando Linux lista os arquivos de um diretório?",
  options: ["ls", "pwd", "cd", "mkdir"],
  answer: 0,
  explanation: "O comando 'ls' lista os arquivos e pastas do diretório atual."
},

Instruções para inserir:
Insira novas perguntas antes do fechamento do array ]; na variável QUESTIONS.

Mantenha o formato correto, especialmente as vírgulas entre os objetos.

Use level para definir se a questão é intermediária ou avançada.

Certifique-se que o índice answer corresponde à posição correta da resposta no array options (começa em zero).

```

## Sugestões para expansão
Você pode criar questões específicas das suas áreas de estudo: cibersegurança, governança de dados, redes, Linux, programação, DevOps, etc.

Também é possível adaptar o código para importar as perguntas de um arquivo JSON externo.

Integrar com frameworks JS para adicionar funcionalidades mais avançadas (React, Vue, etc).

## Tecnologias utilizadas
HTML5, CSS3 e JavaScript puro (ES6+).

Funciona em qualquer navegador moderno, sem dependências externas.


## Feedback e melhorias
Caso queira sugerir melhorias, adicionar funcionalidades ou reportar bugs, fique à vontade para abrir issues ou pull requests neste repositório.

## Autor
André Gonçallez
LinkedIn | GitHub

## Licença
Este projeto é livre para uso, adaptação e compartilhamento.

