# OrVex-Navegador-
Navegador de baixo consumo, navegador compatível com processador 32bits e 64bits esse navegador e leve e prático para Android e tem seu próprio bloqueador de anúncios. 

# OrVex Browser

<p align="center">
  <img src="store/orvex_icon_512.png" width="140" alt="OrVex Browser">
</p>

<h1 align="center">OrVex</h1>

<p align="center">
  Um navegador Android leve, rápido e focado em privacidade,
  desempenho e controle do usuário.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-5.0%2B-green?logo=android">
  <img src="https://img.shields.io/badge/Version-0.19.0-blue">
  <img src="https://img.shields.io/badge/Architecture-32%20%26%2064%20bits-purple">
  <img src="https://img.shields.io/badge/Status-Experimental-orange">
</p>

---

## Sobre o OrVex

O OrVex é um navegador desenvolvido para Android com foco em oferecer uma experiência de navegação leve, funcional e personalizável.

O projeto foi desenvolvido com uma proposta simples: oferecer recursos importantes de um navegador moderno sem depender de dezenas de bibliotecas pesadas ou consumir recursos desnecessariamente.

O OrVex utiliza o Android System WebView como motor de navegação, aproveitando a tecnologia já disponível no próprio sistema.

O navegador foi projetado para funcionar tanto em dispositivos Android de 32 bits quanto de 64 bits.

## Principais funcionalidades

### Navegação

- Navegação por múltiplas abas.
- Gerenciamento de abas.
- Restauração de sessões.
- Barra de endereço e pesquisa.
- Atalhos na nova aba.
- Favoritos.
- Histórico de navegação.
- Navegação em tela cheia.
- Suporte a links externos.
- Interface em português e inglês.

### Gerenciamento inteligente de memória

O OrVex utiliza uma arquitetura otimizada para reduzir o consumo de recursos.

- Mantém apenas um WebView ativo durante a navegação normal.
- Abas inativas preservam seu estado quando possível.
- Novas abas não precisam criar imediatamente um WebView.
- Estados de abas podem ser descartados quando o Android sinaliza pressão de memória.
- Redução de processamento desnecessário em segundo plano.

O objetivo é proporcionar uma navegação mais eficiente, inclusive em aparelhos com recursos limitados.

### Downloads

Um dos principais recursos do OrVex é seu sistema integrado de downloads.

Suporta diferentes categorias de arquivos:

- Vídeos.
- Imagens.
- Aplicativos APK.
- Documentos PDF.
- Arquivos ZIP, RAR e outros compactados.
- Arquivos de áudio.
- Arquivos de texto.
- Outros formatos disponibilizados por HTTP/HTTPS.

Recursos disponíveis:

- Downloads simultâneos, com limite de três transferências HTTP/HTTPS.
- Barra de progresso.
- Velocidade de download.
- Pausar e retomar transferências HTTP compatíveis.
- Cancelar downloads.
- Tentar novamente downloads com falha.
- Histórico de downloads.
- Escolha da pasta de destino.
- Identificação de nomes e extensões dos arquivos.
- Notificações de transferência.
- Suporte a links Blob e Data em condições compatíveis.

O sistema também possui mecanismos para evitar conflitos entre arquivos com nomes iguais.

**Vídeos e streaming:**

O OrVex possui suporte experimental para montagem de determinados vídeos HLS VOD não protegidos, desde que utilizem segmentos compatíveis.

HLS protegido, transmissões ao vivo, DRM e determinados formatos de streaming não são suportados pelo mecanismo de montagem.

### Bloqueador de anúncios

O navegador possui um sistema próprio de bloqueio de anúncios e elementos intrusivos.

Entre os recursos:

- Bloqueio de domínios conhecidos de publicidade.
- Proteção contra rastreadores de terceiros.
- Bloqueio de determinados pop-ups.
- Proteção contra redirecionamentos suspeitos.
- Filtros cosméticos para elementos publicitários.
- Ocultação opcional de determinados avisos de cookies.
- Proteção opcional contra widgets sociais incorporados.
- Listas adicionais de filtros.
- Regras personalizadas.
- Estatísticas de bloqueio.
- Configurações individuais por site.

O usuário pode desativar a proteção em sites específicos caso algum recurso deixe de funcionar.

O bloqueador utiliza um mecanismo próprio e interpreta um subconjunto das regras EasyList/Adblock Plus. Não é um motor completo de compatibilidade ABP.

### Navegação privada

O OrVex possui uma janela de navegação privada com isolamento de processo e diretório de dados WebView próprio em Android 9 ou superior.

Características:

- Perfil separado da navegação normal.
- Cookies isolados.
- Histórico privado não restaurado.
- Limpeza de dados locais cobertos pelas APIs disponíveis do Android.
- Bloqueio de capturas de tela enquanto a janela privada está em primeiro plano.

**Importante:** navegação privada não significa anonimato na internet. Provedores, sites e serviços de rede ainda podem observar determinadas atividades. Também não é possível garantir a eliminação absoluta de todos os dados internos do WebView.

### Proteção de navegação

O OrVex utiliza recursos de segurança disponíveis no Android System WebView.

Inclui:

- Safe Browsing quando disponível.
- Avisos para possíveis páginas de phishing e malware identificadas pelo serviço.
- Análise heurística de URLs suspeitas.
- Detecção de determinados padrões de endereços potencialmente perigosos.
- Comportamento seguro diante de erros de certificados SSL.

Esses mecanismos não substituem um antivírus e não realizam uma análise completa do código ou dos arquivos de todos os sites.

### Reprodução de vídeos

- Reprodução utilizando o Android System WebView.
- Suporte aos formatos disponibilizados pelo WebView e pelos codecs do aparelho.
- Tela cheia.
- Modo Picture-in-Picture (PiP).
- Compatibilidade com players HTML5.
- Diagnóstico de determinadas falhas de reprodução e carregamento de mídia.

A compatibilidade com HLS, DASH e outros formatos depende do player, do WebView e dos codecs disponíveis no dispositivo.

### Personalização

- Imagem de fundo personalizada na nova aba.
- Atalhos de navegação.
- Configurações do bloqueador.
- Preferências de proteção por site.

---

## Desempenho e compatibilidade

O OrVex foi desenvolvido com prioridade para baixo consumo de memória e processamento.

**Requisitos:**

| Recurso | Compatibilidade |
|---|---|
| Sistema | Android 5.0 ou superior |
| Arquitetura | 32 e 64 bits |
| Motor | Android System WebView |
| Linguagem principal | Kotlin |
| Java | 17 |
| SDK de compilação | Android 35 |

O mesmo APK foi configurado para suportar arquiteturas de 32 e 64 bits, sem bibliotecas nativas próprias.

O desempenho depende também do hardware, da versão do Android System WebView e dos recursos do dispositivo.

## Privacidade

O OrVex busca reduzir a coleta e a retenção desnecessária de informações locais.

- Não possui sistema próprio de contas.
- A navegação privada utiliza perfil separado.
- As estatísticas do bloqueador são armazenadas localmente.
- O diagnóstico de mídia não registra URLs completas nem cookies.
- O usuário controla as exceções de proteção por site.

A privacidade também depende dos sites acessados, dos serviços utilizados e do próprio sistema Android.

---

## Versão atual

**OrVex 0.19.0 — Fase 19**

Esta versão concentra melhorias no sistema de downloads, identificação individual de vídeos, tratamento de nomes de arquivos e compatibilidade com determinados streams HLS VOD.

Também inclui correções para evitar que downloads diferentes sejam apresentados como se fossem o mesmo arquivo.

## Instalação

1. Acesse a seção **Releases** deste repositório.
2. Baixe o APK disponibilizado.
3. Abra o arquivo no Android.
4. Autorize a instalação quando o sistema solicitar.

O Android pode solicitar autorização para instalar aplicativos provenientes de fontes externas.

## Limitações conhecidas

O OrVex continua em desenvolvimento.

Algumas limitações importantes:

- Nem todos os anúncios podem ser bloqueados.
- Alguns sites podem detectar o bloqueador.
- A navegação privada não garante anonimato absoluto.
- Alguns sites podem apresentar incompatibilidade com o WebView.
- DRM e determinados sistemas de streaming não são suportados pelo mecanismo de download.
- HLS VOD possui restrições de compatibilidade.
- A reprodução depende dos codecs disponíveis no dispositivo.
- Alguns downloads dependem de autenticação, cookies e suporte do servidor.

## Distribuição

Este repositório disponibiliza o README e os arquivos APK do OrVex.

O código-fonte do projeto não está disponibilizado publicamente neste repositório.

## Feedback

Encontrou algum problema, incompatibilidade ou comportamento inesperado?

Você pode utilizar a seção **Issues** deste repositório para relatar problemas e sugerir melhorias.

Relatos com informações sobre o modelo do aparelho, versão do Android e descrição do problema ajudam bastante.

---

<p align="center">
  <b>OrVex Browser</b>
  <br>
  Navegue com liberdade. Use menos recursos.
</p>
