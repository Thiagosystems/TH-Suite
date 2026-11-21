<p align="center">
  <img src="docs/logo.png" alt="TH Suite" width="220">
</p>

<h1 align="center">TH Suite</h1>

<p align="center">
  Otimização completa para Windows em um só app: otimizador, memória RAM, limpeza, desinstalador, hardware, internet para jogos, segurança e reparos.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/.NET-8-512BD4?logo=dotnet" alt=".NET 8">
  <img src="https://img.shields.io/badge/licen%C3%A7a-MIT-green" alt="Licença MIT">
</p>

<p align="center"><a href="README.md">🇺🇸 Read in English</a></p>

---

O TH Suite junta o **TH Reduct**, o **TH Cleaner**, o **TH Control** e o **TH Guard** com um **otimizador do Windows** e uma central de **reparos**. Tudo explicado em português simples: cada opção diz o que faz, quando vale a pena e quando não usar.

## ✨ Recursos

### 🏠 Início
- **Nota de saúde do PC** (memória, disco, ajustes pendentes e segurança) com atalho para resolver cada problema
- **Otimização rápida** com um clique: ponto de restauração, RAM, arquivos inúteis, ajustes seguros e DNS
- Uso de CPU, RAM, disco e status do antivírus em tempo real
- Informações do PC: Windows, processador, placa de vídeo, memória, placa-mãe e tempo ligado

### ⚡ Otimizador (mais de 80 ajustes)
- **Desempenho**: efeitos visuais, prioridade do programa em primeiro plano, SysMain/Prefetch, indexação, compressão de memória, relatórios de erro e mais
- **Jogos**: Modo de Jogo, Game DVR, Game Bar, otimizações de tela cheia, prioridade de CPU/GPU (MMCSS), aceleração do mouse, Teclas de Aderência, Xbox, Isolamento de Núcleo e VBS
- **Energia**: plano Desempenho Máximo, suspensão de USB, PCIe, Core Parking, Power Throttling/EcoQoS, hibernação e Inicialização Rápida
- **Placa de vídeo**: HAGS, MPO, TDR, telemetria NVIDIA e ULPS da AMD (só aparece o que serve para a sua placa)
- **Rede**: limitação de rede, economia de energia da placa de rede, Otimização de Entrega e Teredo
- **Privacidade**: telemetria do Windows, Office, navegadores e Visual Studio, ID de publicidade, histórico de atividades, Recall e SMBv1
- **Windows 11**: sem anúncios no Iniciar, pesquisa sem Bing, Widgets, Copilot, menu de contexto clássico, barra à esquerda, "Finalizar tarefa" e mais
- **Serviços** e **Windows Update** com aviso claro do que deixa de funcionar
- Cada ajuste tem **nível de risco**, explicação completa, aviso de notebook e de reinício
- Nada muda antes de clicar em **Aplicar**; o valor original de tudo fica guardado e **qualquer ajuste pode ser desfeito**
- **Ponto de restauração automático** antes de aplicar
- **Remover apps inúteis** (Notícias, Clipchamp, Candy Crush, Teams pessoal...) sem tocar nos essenciais

### 🧠 Memória RAM
- Limpeza de working set, cache do sistema, páginas modificadas e lista standby
- Limpeza automática por uso ou intervalo, avisos de RAM alta e de app pesado
- **Modo jogo**: prioridade para o jogo, plano de energia, pausar ou fechar apps pesados, detecção da Steam, Epic e Riot
- Widget por cima dos jogos, atalho de teclado global e histórico

### 🧹 Limpeza e desinstalação
- Temporários do Windows, caches de navegadores e apps, lixeira, logs e mais
- Arquivos grandes, desinstalador completo com **remoção de sobras** e backup do registro, apps da Store

### 🌡️ Hardware e internet
- Temperaturas, uso, clock, consumo, discos e ventoinhas (LibreHardwareMonitor)
- Perfis de ventoinha e energia: silencioso, equilibrado e desempenho
- **Internet para jogos**: teste e troca de DNS, Nagle, limitação de rede e prioridade (QoS) para jogos

### 🛡️ Segurança
- Verificação inteligente + Microsoft Defender + VirusTotal (opcional)
- **Detecção de mineradores** escondidos, processos disfarçados, extensão dupla e inicialização suspeita
- Exclusões do Defender, hosts, proxy, firewall, quarentena reversível e monitor em tempo real

### 🔧 Reparos e ferramentas
- 31 reparos explicados: internet, DNS, Wi-Fi, modo avião, Bluetooth, áudio, microfone, câmera, impressora, hora, arquivos corrompidos (DISM + SFC), DLLs (Visual C++ e DirectX), disco, Windows Update, Menu Iniciar, Explorador, ícones, copiar e colar, tela preta, PC que não desliga, Windows Installer, PIN, Store, apps do Windows, Xbox, Defender, pesquisa, CPU, RAM e disco em 100%
- O resultado aparece ao vivo
- Ferramentas rápidas: ponto de restauração, reiniciar o Explorador, reiniciar na BIOS ou no modo de recuperação e atalhos do Windows

### 🎨 Personalização
- Temas escuro, preto e claro, cores de destaque e **cor da logo**
- Fica na bandeja com a % da RAM no ícone, inicia com o Windows

## 📥 Download

Baixe a versão mais recente em [**Releases**](https://github.com/Thiagosystems/THSuite/releases).

> Não precisa instalar nada: o .exe já inclui o .NET. Funciona no Windows 10/11 64 bits e pede permissão de **administrador**.

## 🛠️ Compilar

Pré-requisito: [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)

```bat
git clone https://github.com/Thiagosystems/THSuite.git
cd THSuite
build.bat
```

O executável fica em `publish\THSuite.exe`.

## 📁 Estrutura

| Pasta / arquivo | Função |
|---|---|
| `MainWindow`, `HomeView`, `SettingsView` | Janela, tela inicial e configurações |
| `Core/` | Tema, logo, bandeja, comandos e início com o Windows |
| `Modules/Optimizer/` | Otimizador (`Catalog.cs` tem todos os ajustes) e remoção de apps |
| `Modules/Memory/` | Limpeza de RAM e modo jogo |
| `Modules/Cleaner/` | Limpeza de disco e desinstalador |
| `Modules/Hardware/` | Sensores, ventoinhas, energia e internet |
| `Modules/Security/` | Vírus, mineradores, inicialização e quarentena |
| `Modules/Repair/` | Reparos (`Fixes.cs`) e ferramentas |

## ⚠️ Avisos

- Ajustes marcados como **Avançado** reduzem segurança ou desligam recursos; leia o aviso antes.
- Crie um ponto de restauração (o TH Suite faz isso sozinho por padrão).
- Heurísticas de segurança podem gerar falsos positivos.

## 📄 Licença

Distribuído sob a licença MIT. Veja [LICENSE](LICENSE). Bibliotecas de terceiros em [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
