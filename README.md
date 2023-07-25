# cronometro-js
Stopwatch with + HTML +CSS + JAVASCRIPT
Este código é uma implementação simples de um cronômetro utilizando HTML, CSS e JavaScript. Vamos fazer uma pequena descrição das principais partes do código:

Variáveis e elementos DOM: As primeiras linhas do código definem variáveis para os elementos do DOM (Document Object Model) que serão manipulados para exibir os valores do cronômetro. Os elementos são representados pelas constantes minutesEl, secondsEl e millisecondsEl, que correspondem às tags HTML com os IDs "minutes", "seconds" e "milliseconds", respectivamente. Além disso, existem botões para controlar o cronômetro: startBtn, pausetBtn, resumeBtn e resetBtn.

Variáveis do cronômetro: Em seguida, são definidas variáveis relacionadas ao cronômetro, como interval, que armazenará o ID do intervalo de atualização, e as variáveis minutes, seconds e milliseconds, que armazenam os valores do cronômetro em minutos, segundos e milissegundos, respectivamente. Também há uma variável isPaused, que controla o estado de pausa do cronômetro.

Event Listeners: São adicionados event listeners (ouvintes de eventos) aos botões para que o cronômetro possa ser controlado pelo usuário. Quando o botão "startBtn" é clicado, a função startTimer() é chamada para iniciar o cronômetro. Da mesma forma, os botões "pauseBtn" e "resumeBtn" têm suas próprias funções pauseTime() e resumeTimer() para pausar e continuar o cronômetro, respectivamente. O botão "resetBtn" chama a função resetTimer(), que redefine o cronômetro para o estado inicial.

Função startTimer(): Essa função inicia o intervalo de atualização do cronômetro usando setInterval(). A cada 10 milissegundos, a função interna é executada. Se o cronômetro não estiver pausado (isPaused é falso), os valores de milissegundos, segundos e minutos são atualizados de acordo. Os valores são exibidos nos elementos do DOM correspondentes usando as funções formatTime() e formatMilliseconds().

Funções pauseTime() e resumeTimer(): Essas funções são chamadas quando os botões de pausa e continuar são clicados, respectivamente. Elas atualizam a variável isPaused para controlar o estado de pausa do cronômetro e também ajustam a exibição dos botões no DOM para mostrar o botão apropriado.

Função resetTimer(): Quando o botão de redefinir é clicado, esta função é acionada. Ela limpa o intervalo de atualização usando clearInterval(), redefine as variáveis do cronômetro e atualiza a exibição dos elementos no DOM para os valores iniciais.

Funções de formatação: As funções formatTime() e formatMilliseconds() são usadas para garantir que os valores exibidos no cronômetro sempre tenham dois dígitos para minutos e segundos e três dígitos para milissegundos.

No geral, esse código cria um cronômetro simples que pode ser iniciado, pausado, continuado e redefinido pelo usuário através dos botões. Os valores de minutos, segundos e milissegundos são exibidos e atualizados dinamicamente no DOM.

![cronometro-javascript](https://github.com/JohnatanChagas/cronometro-js/assets/127504003/be59a9fd-8f63-4b43-9cf1-5608c0f15d93)
