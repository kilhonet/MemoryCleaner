# MemoryCleaner

**Limpador de memória leve e gratuito para Windows: libera memória com um clique e limpa sozinho nas condições que você definir.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · Português (Brasil) · [Français](README.fr.md)

> Este documento é uma tradução. Em caso de divergência, a [versão em coreano](README.ko.md) prevalece.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
![Version](https://img.shields.io/badge/version-3.0.0-blue)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/memorycleaner?lang=pt)

![Tela do MemoryCleaner](images/memorycleaner-en.webp)

> O programa não tem tradução para português; ele é exibido em inglês. Os nomes de botões e menus abaixo aparecem como na tela.

## Visão geral

O MemoryCleaner mostra quanta memória está em uso agora e, com um só clique em **Clean memory**, recupera o cache que o Windows mantém guardado e a memória que os programas abertos não estão usando no momento.

Você pode configurá-lo para limpar sozinho quando o uso de memória fica alto, em intervalos fixos, ou quando o cache se acumula e falta memória livre. Enquanto um jogo ou vídeo roda em tela cheia, ele pula a limpeza para não atrapalhar.

Ao fechar a janela, ele vai para a área de notificação (bandeja do sistema) e continua trabalhando em silêncio. Depois que a janela fecha, o MemoryCleaner libera também toda a memória que ela usava, então, esperando na bandeja, ocupa só cerca de 1 MB.

## Principais recursos

- **Limpeza com um clique** — Limpe a memória com o botão **Clean memory** ou com um só clique no ícone da bandeja.
- **Escolha o que limpar** — Escolha você mesmo as áreas: cache de arquivos, conjunto de trabalho, lista de espera, cache do registro, combinação de memória e mais.
- **Limpeza automática** — Limpa quando o uso da memória física · virtual · do conjunto de trabalho passa de um limite, ou em intervalos fixos.
- **Anti-travadas em jogos** — Quando o cache (a lista de espera) se acumula e falta memória livre, esvazia só o cache.
- **Detecção de tela cheia** — Pula a limpeza automática enquanto um jogo, vídeo ou apresentação está em tela cheia.
- **Estado da memória** — Veja memória física, memória virtual, conjunto de trabalho e cache na tela inicial e no ícone da bandeja.
- **Leve** — Um único executável que usa só cerca de 1 MB enquanto espera na bandeja.
- **9 idiomas** — Coreano · inglês · japonês · chinês · russo · italiano · francês · espanhol · árabe.

## Download / Instalação

| Tipo | Link |
|---|---|
| Instalador | [Download](https://down.kilho.net/memorycleaner?lang=pt) |
| Portátil (ZIP) | [Download](https://down.kilho.net/memorycleaner?lang=pt&nosetup) |

O instalador abre o MemoryCleaner assim que a instalação termina e ativa **Run on system start**, para que ele inicie na bandeja toda vez que você entrar no Windows. Na versão portátil, descompacte o ZIP e execute `MemoryCleaner.exe`. As duas versões têm os mesmos recursos.

Limpar a memória exige direitos de administrador, então o Windows mostra um pedido de permissão ao executar. Clique em **Sim**.

## Como usar

### Primeiros passos

1. Execute o MemoryCleaner e clique em **Sim** no pedido de permissão de administrador.
2. **Home** mostra o uso da memória física em barra e números, com memória virtual · conjunto de trabalho · cache logo abaixo. Os valores são atualizados a cada segundo.
3. Clique em **Clean memory**; o botão muda para **Cleaning** e, quando termina, você já vê o uso menor.
4. Para que ele limpe sozinho, clique em **Config** e ative as condições que quiser em **Auto clean**.
5. Fechar a janela mantém o MemoryCleaner rodando na bandeja. Clique no ícone para abrir a janela de novo.

### Organização da tela

**Botões de cima**

| Elemento | Função |
|---|---|
| **Home** | A tela principal, com o estado da memória e o botão **Clean memory** |
| **Config** | Auto clean · Clean targets · General |
| **Donate** | Abre a página de doação |
| Logotipo KILHO.net | Abre a página de apresentação do MemoryCleaner |

**Home**

| Elemento | Conteúdo |
|---|---|
| Barra | Uso da memória física |
| **Physical** | Usada / total (MB) e porcentagem de uso |
| **Virtual** | Uso da memória virtual, incluindo o arquivo de paginação |
| **working set** | Memória ocupada pelos programas abertos, e sua proporção |
| **Cached** | Memória que o Windows guarda como cache (o mesmo valor de "Em cache" no Gerenciador de Tarefas) e sua proporção da memória física |
| **Clean memory** | Limpa na hora. Muda para **Cleaning** enquanto trabalha |

**Config**

| Grupo | Itens |
|---|---|
| **Auto clean** | **Clean when physical memory usage is higher than (%)** · **Clean when pagefile usage is higher than (%)** · **Clean when total workingset usage is higher than (%)** · **Clean automatically if interval (minutes) exceeded.** · **Purge cached (standby list) memory (anti-stutter)** · **Skip cleaning in full screen** |
| **Clean targets** | **File cache** · **working set** · **Standby list (low priority)** · **Registry cache** · **Combine memory** · **Standby list \*** · **Modified page list \*** |
| **General** | **Run on system start** · **Clean when you click on the task icon** |
| Embaixo | Versão atual e botão **Defaults** |

**Ícone da bandeja**

| Ação | Resultado |
|---|---|
| Passar o mouse | Uso da memória física · virtual · do conjunto de trabalho |
| Clique esquerdo | Abre a janela (limpa na hora se **Clean when you click on the task icon** estiver ativado) |
| Clique direito | **MemoryCleaner** (abrir a janela) · **Crafted by Kilho** (página de apresentação) · **Quit** |

Durante a limpeza, o ícone da bandeja muda de aparência, então você sabe que ele está trabalhando sem abrir a janela.

**Clean targets** — o que cada um libera

| Item | O que libera | Padrão |
|---|---|---|
| **File cache** | O cache que o Windows acumula ao ler e gravar arquivos | Ativado |
| **working set** | A memória que os programas abertos não estão usando no momento | Ativado |
| **Standby list (low priority)** | A parte do cache com menos chance de ser usada de novo | Ativado |
| **Registry cache** | O cache acumulado ao ler o registro | Ativado |
| **Combine memory** | Junta conteúdos de memória idênticos em um só para liberar espaço | Ativado |
| **Standby list \*** | Todo o cache | Desativado |
| **Modified page list \*** | A memória esperando para ser gravada no disco | Desativado |

Os itens marcados com `*` podem causar travadinhas breves em jogos ou ao reproduzir vídeo, por isso vêm desativados.

### O que fazer quando…

**Quer limpar a memória agora**
Clique em **Clean memory** na **Home**. O botão muda para **Cleaning** enquanto trabalha e volta para **Clean memory** ao terminar. Clique quando o PC estiver pesado depois de muitos programas abertos por muito tempo, ou logo antes de abrir um jogo grande ou um programa de edição.

**Quer limpar pelo ícone da bandeja sem abrir a janela**
Ative **Config → Clean when you click on the task icon** e um só clique no ícone da bandeja limpa a memória. Ao terminar, aparece a notificação "Optimized memory.". Enquanto essa opção estiver ativada, abra a janela clicando com o botão direito no ícone → **MemoryCleaner**.

**Quer ver o estado da memória sem a janela**
Passe o mouse sobre o ícone da bandeja para ver o uso da memória física · virtual · do conjunto de trabalho — o bastante para saber se precisa limpar sem abrir a janela.

**Quer que ele limpe sozinho quando faltar memória**
Em **Config → Auto clean**, ative **Clean when physical memory usage is higher than (%)** e escolha um limite (30 – 90%) na caixa ao lado. Quando o uso passar do limite, o MemoryCleaner limpa sozinho. Se você usa muito o arquivo de paginação, ative também **Clean when pagefile usage is higher than (%)**; se o problema são programas que ocupam muita memória, ative **Clean when total workingset usage is higher than (%)**. Quando a limpeza não faz o uso cair, ele espera antes de limpar de novo em vez de repetir sem parar, para que a limpeza não vire um peso.

**Quer limpar em intervalos regulares**
Ative **Clean automatically if interval (minutes) exceeded.** e escolha 5 · 10 · 20 · 30 · 40 · 50 · 60 minutos: ele limpa nesse intervalo, qualquer que seja o uso. Bom para manter leve um PC que fica ligado por muito tempo.

**Um jogo fica cada vez mais travado quanto mais você joga (esvaziar o cache)**
Às vezes um jogo trava cada vez mais com o tempo, até que só reiniciar o jogo resolve. Isso acontece porque o Windows guarda como cache (a lista de espera) os arquivos que já leu; quando esse cache se acumula e a memória livre acaba, o Windows precisa recuperá-lo às pressas, e o jogo congela por um instante. Ative **Purge cached (standby list) memory (anti-stutter)**: quando o cache passar do limite **Purge when cached (MB) is higher than** (512 · 1024 · 2048 · 4096 MB) e, ao mesmo tempo, a memória livre ficar abaixo do limite **Purge when free memory (MB) is lower than** (1024 · 2048 · 4096 · 8192 · 16384 MB), ele esvazia só o cache antes. Só age quando as duas condições são atendidas, e depois de esvaziar elas se desfazem sozinhas, então ele só entra em ação quando é preciso.

O ideal é definir o limite de memória livre como metade da memória instalada no seu PC.

| Memória instalada | Purge when free memory (MB) is lower than |
|---|---|
| 8 GB | 4096 (padrão) |
| 16 GB | 8192 |
| 32 GB | 16384 |

Não precisa ativar só na hora de jogar. Ele usa cerca de 1 MB na bandeja e só age quando as condições são atendidas, então pode deixar ativado.

**Quer que ele não mexa em nada durante um jogo ou filme**
**Skip cleaning in full screen** já vem ativado. Enquanto um jogo, vídeo ou apresentação estiver em tela cheia, a limpeza automática é pulada para evitar travadas. Ao sair da tela cheia, volta a funcionar normalmente.

**Quer escolher você mesmo as áreas a limpar**
Marque as áreas em **Config → Clean targets**. Tanto o botão **Clean memory** quanto a limpeza automática seguem essa escolha. Se nada estiver marcado, não há o que fazer e o botão **Clean memory** fica acinzentado.

**Quer uma limpeza mais forte**
Ativar **Standby list \*** e **Modified page list \*** libera também todo o cache e a memória esperando gravação, o que mais libera memória. Mas isso pode causar travadinhas breves em jogos ou vídeos, então ative só quando precisar e deixe desativado no dia a dia.

**Quer saber o que é "Cached"**
**Cached** na **Home** é a memória que o Windows guarda para o caso de precisar de novo — o mesmo valor de "Em cache" no Gerenciador de Tarefas. Um valor alto não é ruim por si só, mas se os jogos travarem, experimente ativar o esvaziamento do cache acima.

**Quer que ele inicie com o Windows**
Ative **Config → Run on system start** e, pouco depois de você entrar no Windows, o MemoryCleaner inicia em silêncio na bandeja — sem pedido de permissão de administrador. Na versão instalada já vem ativado.

**Quer que ele continue rodando depois de fechar a janela**
O X da janela não fecha o MemoryCleaner: ele vai para a bandeja e continua a limpeza automática. Ele também libera toda a memória que a janela usava, então deixá-lo rodando quase não custa nada. Para sair de vez, clique com o botão direito no ícone da bandeja → **Quit** e confirme.

**Sai enquanto ele está limpando**
Se você sair durante uma limpeza, o botão muda para **Exit after cleaning** e o programa fecha quando a limpeza termina. A limpeza nunca é cortada no meio.

**Quer voltar tudo ao padrão**
Clique em **Defaults** na parte de baixo de **Config** e confirme: todas as opções de limpeza automática e de áreas a limpar voltam ao padrão. **Run on system start** não é alterado.

**Executa de novo quando ele já está rodando**
Só um MemoryCleaner roda por vez. Se você executar de novo enquanto ele está na bandeja, não abre outro: abre a janela do que já está rodando.

## Configuração

Cada configuração é salva assim que você a muda e usada de novo na próxima execução.

| Item | Padrão |
|---|---|
| Limpeza pelo uso da memória física · arquivo de paginação · conjunto de trabalho | Off (limite de 90% ao ativar) |
| Clean automatically if interval (minutes) exceeded. | Off (30 minutos ao ativar) |
| Purge cached (standby list) memory | Off (cache ≥ 1024 MB · memória livre < 4096 MB ao ativar) |
| Skip cleaning in full screen | On |
| Clean targets | File cache · working set · Standby list (low priority) · Registry cache · Combine memory |
| Run on system start | On na versão instalada |
| Clean when you click on the task icon | Off |
| Idioma | Segue a configuração de região do Windows (inglês quando o idioma não é suportado) |

## Requisitos

- Windows 10 · Windows 11 (64 bits)
- Direitos de administrador — necessários para limpar a memória. Aparece um pedido de permissão ao executar (mas não quando ele inicia por **Run on system start**).
- Nenhum outro componente para instalar.
- A conexão com a internet é usada só para avisos de nova versão.

## Atualizações

O MemoryCleaner **não** se atualiza sozinho. Ao iniciar, ele verifica se há uma nova versão e mostra um aviso; clicar em **[Yes]** abre a página de download e fecha o programa. As novas versões são publicadas manualmente após testes internos e anunciadas na [página do MemoryCleaner](https://kilho.net/memorycleaner). Veja o [aviso sobre a política de atualização](https://en.kilho.net/archives/notice/2940).

**Histórico de versões**

| Versão | Data | Mudanças |
|---|---|---|
| 3.0.0 | 2026-09-29 | Refeito do zero em C puro, mais rápido e estável — memória em espera na bandeja reduzida em mais de 95% e tamanho do programa em cerca de 98%, escolha das áreas a limpar, esvaziamento automático do cache (anti-travadas em jogos), cache exibido na tela inicial, configurações de limpeza padrão pensadas para jogos e vídeo, botão para restaurar o padrão, verificação de atualizações e inicialização mais confiáveis |
| 2.0.3 | 2026-09-03 | Melhor detecção de tela cheia para não interromper jogos e vídeos, encerramento mais estável, avisos de conclusão mais precisos, limpezas repetidas otimizadas, configurações mais estáveis |
| 2.0.2 | 2026-08-13 | Opção para pular a limpeza em tela cheia, configuração de início automático removida na desinstalação, carregamento das configurações e início automático mais confiáveis |
| 2.0.1 | 2026-07-13 | Limpeza da memória de navegadores reforçada, mais estabilidade em uso prolongado, avisos e configurações mais confiáveis, espanhol adicionado |

## Licença

O MemoryCleaner é **freeware**. Pode ser usado de graça e sem restrições em qualquer lugar — no trabalho, em casa, em órgãos públicos ou na escola — e redistribuído livremente.

## Links

- Site: <https://kilho.net/memorycleaner>
- Fórum: <https://groups.google.com/g/kilhonet>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
