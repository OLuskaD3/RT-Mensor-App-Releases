<div align="center">

# RT Mensor — Instaladores Oficiais

**Distribuição pública dos instaladores assinados do RT Mensor**

[![Última versão](https://img.shields.io/github/v/release/OLuskaD3/RT-Mensor-App-Releases?style=flat-square&label=última%20versão)](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/OLuskaD3/RT-Mensor-App-Releases/total?style=flat-square)](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases)
[![Plataforma](https://img.shields.io/badge/Windows-10%2B-blue?style=flat-square&logo=windows)](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases/latest)

</div>

---

##  Download da última versão

 **[Baixar instalador mais recente](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases/latest)**

Procure o arquivo `RT.Mensor_X.Y.Z_x64-setup.exe` e execute. Após a
primeira instalação, o aplicativo se atualiza automaticamente em até
4 horas após cada nova versão publicada.

---

##  Sobre este repositório

**Este repositório contém apenas binários compilados** — não há
código-fonte aqui. Cada release inclui:

| Arquivo | Descrição |
|---|---|
| `RT.Mensor_X.Y.Z_x64-setup.exe` | Instalador NSIS para Windows x86_64 |
| `RT.Mensor_X.Y.Z_x64-setup.exe.sig` | Assinatura digital Ed25519 do `.exe` |
| `latest.json` | Manifesto para o updater automático |

Todos os instaladores são **assinados digitalmente**. O próprio
aplicativo verifica a assinatura antes de aplicar uma atualização —
qualquer adulteração do `.exe` durante o download é rejeitada.

---

##  Segurança

A chave pública usada para verificar as assinaturas vem **embutida**
no próprio aplicativo. Cenários de ataque cobertos:

- ✅ **MITM no download** → assinatura do `.exe` não bate → app recusa
- ✅ **Este repositório comprometido** → idem
- ✅ **Atacante rouba chave pública** → não há nada que ele faça (é pública)

A chave privada de assinatura mora **fora deste repositório**, sob
custódia da Mênsor & Martins.

---

##  Onde NÃO procurar suporte aqui

- **Não há issues abertas** para uso do aplicativo neste repositório
  público (público mas não-colaborativo).
- **Dúvidas operacionais** → entre em contato pelos canais internos
  da Mênsor & Martins.
- **Bugs e sugestões** → reportados no repositório privado de
  desenvolvimento (acesso restrito).

---

##  Histórico de versões

O histórico completo de mudanças está disponível na seção
[Releases](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases)
e nas notas de cada versão.

Para o CHANGELOG técnico detalhado, consulte o repositório de
desenvolvimento (acesso restrito).

---

<div align="center">

**Mênsor & Martins** · Inteligência Tributária · © 2026

</div>
