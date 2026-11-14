# Robô do ProfeX

Programa para Windows que passa para o **SIAGE**, sozinho, o que você já lançou no **ProfeX**: frequência, registro de aula e notas. Ele fica perto do relógio do Windows e trabalha quando você clica em **Enviar ao SIAGE** no ProfeX (no computador ou no celular), desde que o computador esteja ligado.

## Antes de instalar

- Computador com **Windows 10 ou 11** e o **Microsoft Edge** (já vem no Windows).
- Conta no **ProfeX** (https://profe-x.pages.dev) com **"Enviar ao SIAGE" liberado** pelo administrador.
- Suas turmas no ProfeX com **disciplina** preenchida e alunos com os **mesmos nomes** do SIAGE.

## 1. Baixar

Abra **Releases** (à direita nesta página) › versão mais nova › clique em **`ProfeX-Robo-Instalar-x.x.x.exe`**.

O navegador pode avisar *"Este arquivo não é baixado com frequência"*: clique nos **três pontinhos** (ou em **⋯**) › **Manter** › **Manter assim mesmo**.

## 2. Instalar

1. Abra o arquivo baixado.
2. Se aparecer a tela azul **"O Windows protegeu o computador"**: clique em **Mais informações** › **Executar assim mesmo**.
   (O aviso aparece porque o programa não tem assinatura digital paga. Ele é feito por um professor, para professores.)
3. Deixe marcado **"Abrir o robô junto com o Windows"** › **Instalar** › **Concluir**.

Não pede senha de administrador. Se algum **antivírus** reclamar, restaure o arquivo e adicione uma **exceção** para a pasta `%LOCALAPPDATA%\Programs\ProfeX Robo`.

## 3. Configurar (só na primeira vez)

O robô abre um assistente com 3 passos:

1. **Conta do ProfeX:** seu e-mail e senha do ProfeX. A senha **não** fica guardada; o robô guarda só uma chave de acesso no cofre de senhas do Windows.
2. **SIAGE:** endereço (já vem preenchido), seu usuário e senha do SIAGE › **Testar e continuar**. O robô abre o SIAGE no Edge, entra e lê suas turmas. **Não mexa na janela do SIAGE** enquanto ele testa. Se você tiver matrícula em mais de uma escola, escreva parte do nome da escola no campo "Escola".
3. **Ligar as turmas:** confira, para cada turma do ProfeX, qual é a turma do SIAGE (já vem sugerido) › **Salvar e terminar**.

As senhas ficam **só no seu computador** (cofre do Windows). Nada vai para a nuvem.

## 4. Usar

No ProfeX: **Enviar ao SIAGE** › escolha o período, as turmas e o que enviar › botão azul **Enviar ao SIAGE**. O andamento e o resultado aparecem no próprio ProfeX.

O ícone perto do relógio mostra o que o robô está fazendo:

| Cor | Significa |
|---|---|
| 🟢 verde | esperando pedidos |
| 🔵 azul | trabalhando (você vai ver o Edge abrir o SIAGE: não mexa nele) |
| 🔴 vermelho | precisa de atenção (passe o mouse no ícone para ler) |

Clique com o botão direito no ícone para: **Abrir o ProfeX**, **Ver o registro**, **Configurar…**, **Procurar atualização** e **Sair**.

### O que o robô faz e o que NÃO faz

- **Frequência e registro de aula:** grava sozinho os dias que ainda não estão no SIAGE e confere cada um. Dia diferente no SIAGE ele **não** muda: mostra para você decidir.
- **Notas:** só **preenche** caixa vazia ou **aumenta** nota (nunca diminui nem apaga) e salva com **Salvar Parcialmente**. O botão **Lançar notas e Gerar Status** é sempre seu: o robô nunca clica nele.
- Marque **"Só comparar, não gravar"** no ProfeX quando quiser só conferir.

## Atualização

O robô procura versão nova sozinho (ao abrir e a cada 6 horas) e se atualiza sem perguntar, quando não está trabalhando. Também dá para clicar em **Procurar atualização**. Sua configuração continua.

## Problemas

- Clique com o botão direito no ícone › **Ver o registro** e mande o arquivo para quem te indicou o robô (ele **não** tem senhas).
- Teste rápido das peças: menu **Iniciar** › **Testar o Robô do ProfeX**. Aparece uma janelinha com o que está ok e o que deu erro.
- O robô roda pelo **Python oficial** (programa `pythonw.exe`, assinado pela Python Software Foundation), instalado junto, só para ele.

## Desinstalar

**Configurações do Windows › Aplicativos › Robô do ProfeX › Desinstalar.**
