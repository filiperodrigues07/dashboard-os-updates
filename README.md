<div align="center">

# Dashboard OS · Atualizações

**Novas versões do painel de ordens de serviço, prontas para instalar no servidor.**

[![Versão mais recente](https://img.shields.io/github/v/release/filiperodrigues07/dashboard-os-updates?label=vers%C3%A3o%20mais%20recente&color=2563eb)](https://github.com/filiperodrigues07/dashboard-os-updates/releases/latest)
[![Windows](https://img.shields.io/badge/plataforma-Windows-0f172a)](https://github.com/filiperodrigues07/dashboard-os-updates/releases)

[![Baixar atualização 3.4.3](https://img.shields.io/badge/%E2%AC%87%EF%B8%8F_BAIXAR_ATUALIZA%C3%87%C3%83O-3.4.3-2563eb?style=for-the-badge)](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.4.3/DashboardOS-Update-3.4.3.exe)

[Ver todas as versões](https://github.com/filiperodrigues07/dashboard-os-updates/releases) · [Abrir a versão mais recente](https://github.com/filiperodrigues07/dashboard-os-updates/releases/latest)

</div>

> **Já usa o Dashboard OS?** Instale o pacote no **PC servidor**. As estações CLIENT acessam o sistema pelo navegador e não precisam executar este arquivo.

## O que mudou

| Versão | Atualizações | Download |
| :--- | :--- | :--- |
| **[3.4.3](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.4.3)** · mais recente | Corrige o dashboard nas estações e TVs da rede (erro Network Error das versões 3.4.0 e 3.4.1); a atualização agora instala com o servidor em uso, sem travar; o cadastro das situações de OS desativa as situações padrão do banco (A ENTREGAR e ENTREGUE) e cadastra as usadas pelo dashboard; ao fixar o IP do servidor, o DNS passa a ser 8.8.8.8 e 8.8.4.4. | [⬇️ Baixar 3.4.3](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.4.3/DashboardOS-Update-3.4.3.exe) |
| **[3.4.1](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.4.1)** | Correção do firewall do servidor: as TVs/estações voltam a conectar mesmo com a rede marcada como Pública; o instalador agora avisa no final se a regra de firewall não cobre a rede atual. | [⬇️ Baixar 3.4.1](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.4.1/DashboardOS-Update-3.4.1.exe) |
| **[3.4.0](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.4.0)** | Atualização com um clique pelo painel administrativo, com retorno automático à versão anterior se algo falhar; o servidor passa a iniciar com o Windows, sem precisar de login, e a se religar sozinho; as estações CLIENT reconectam sozinhas quando o servidor volta. | [⬇️ Baixar 3.4.0](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.4.0/DashboardOS-Update-3.4.0.exe) |
| **[3.3.6](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.3.6)** | Logo padrão nas telas de acesso e dashboard; colunas da tabela ajustáveis e melhorias na apresentação das ordens de serviço. | [⬇️ Baixar 3.3.6](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.3.6/DashboardOS-Update-3.3.6.exe) |
| **[3.3.5](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.3.5)** | Ajuste da rolagem da tabela pelo painel administrativo; opção de configurar a exclusão do Windows Defender durante a instalação. | [⬇️ Baixar 3.3.5](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.3.5/DashboardOS-Update-3.3.5.exe) |
| **[3.3.4](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.3.4)** | Melhorias na instalação em rede e no visual do instalador; correções na recarga do dashboard e na recuperação da conexão com o Firebird. | [⬇️ Baixar 3.3.4](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.3.4/DashboardOS-Update-3.3.4.exe) |
| **[3.3.3](https://github.com/filiperodrigues07/dashboard-os-updates/releases/tag/v3.3.3)** | Primeira versão com atualização pelo GitHub Releases, verificação de integridade SHA-256 e pacote separado para atualizar uma instalação existente. | [⬇️ Baixar 3.3.3](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.3.3/DashboardOS-Update-3.3.3.exe) |

## Instalação nova

Para instalar o Dashboard OS pela primeira vez, baixe o instalador completo e execute-o **como administrador** no PC servidor:

[⬇️ Baixar instalador completo 3.4.3](https://github.com/filiperodrigues07/dashboard-os-updates/releases/download/v3.4.3/DashboardOS-Setup-3.4.3.exe)

O instalador pergunta se o PC é o **servidor** (onde está o Firebird do CH) ou uma estação/TV (**CLIENT**) e configura banco de dados, atalhos e inicialização automática. As atualizações seguintes são feitas pelo painel administrativo ou pelo ícone da bandeja, sem rodar o instalador de novo.

## Como atualizar

1. No **servidor**, procure o ícone do Dashboard OS na bandeja do Windows, perto do relógio.
2. Quando aparecer **Instalar atualização**, clique nessa opção. O sistema baixa e confere o pacote antes de instalar. A partir da 3.4.0 também é possível atualizar pelo painel administrativo (`http://IP_DO_SERVIDOR:3333/admin`, aba **Atualização**, botão **Atualizar agora**), de qualquer computador da rede.
3. Para instalar manualmente, baixe o `.exe` da versão desejada acima e execute-o no servidor. Confirme a solicitação de administrador do Windows.
4. Ao terminar, abra o Dashboard OS e confira se ele voltou a funcionar normalmente.

O pacote de atualização troca os arquivos do aplicativo e preserva o banco Firebird, o `.env` e as configurações locais. Ele exige uma instalação existente no servidor; para uma instalação nova, use o instalador completo (seção **Instalação nova**).

**Instalações antigas:** servidores nas versões 3.3.0 a 3.3.2 podem instalar manualmente a 3.3.4 ou uma versão posterior se já tiverem `C:\DashboardOS\.env` com `APP_MODE=server` e `launcher.vbs`. Versões anteriores precisam primeiro do instalador completo.

## Sobre os arquivos

Cada release contém `DashboardOS-Update-<versão>.exe` (atualização de um servidor já instalado) e `DashboardOS-Setup-<versão>.exe` (instalador completo, para instalação nova). O código-fonte compactado que o GitHub mostra automaticamente na página da release **não é o instalador**. Para conferir a integridade de um download manual, compare o SHA-256 do arquivo com o `digest` exibido nos detalhes da release.

Os arquivos de configuração do cliente (`.env` e `settings.json`) não são distribuídos neste repositório.
