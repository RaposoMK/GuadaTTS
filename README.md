# GuadaTTS

GuadaTTS é uma TTS para os passa-fomes: uma página estática que acompanha o chat público de um canal da Twitch e lê mensagens que começam com `!m` ou `!msg`.

## Como usar

1. Publique `index.html` em uma hospedagem estática (ou abra em um navegador moderno).
2. Informe o nome do canal no campo e clique em **Conectar**. Também é possível abrir diretamente `index.html?twitch=cellbit`.
3. Envie no chat `!m Olá` ou `!msg Olá`. A página mostra a mensagem e usa a síntese de fala nativa do navegador.
4. Use os controles para ativar/desativar a voz, pular uma fala e escolher se o nome do usuário será lido.
5. Adicione nomes à blacklist; eles continuam aparecendo nos logs, mas não são falados. A lista fica salva no navegador.
6. Clique em **Copiar link para OBS** e adicione o endereço como fonte de navegador. O link gerado usa o formato `?twitch=cellbit&obs_link=true`.

No modo OBS, o fundo é transparente e permanece apenas a última mensagem — incluindo o nome do usuário e a mensagem completa — até que outra mensagem válida seja recebida.

A conexão ao chat público é somente leitura e não pede credenciais. A síntese de fala depende do suporte do navegador/OBS à Web Speech API e das vozes instaladas no sistema. O acesso ao chat depende de a Twitch permitir conexão IRC anônima no canal/rede; a página não envia mensagens.
