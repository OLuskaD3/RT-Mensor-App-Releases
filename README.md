# RT Mensor — Releases

Distribuição oficial dos instaladores do **RT Mensor**, sistema fiscal
desktop da Mênsor & Martins para apuração de PIS/COFINS.

## Download da versão mais recente

[**Baixar instalador (Windows)**](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases/latest)

Clique em "Assets" no release mais recente e baixe o arquivo
`RT.Mensor_<versão>_x64-setup.exe` (~6 MB).

## Como instalar

1. Execute o `.exe` baixado.
2. Aceite o instalador NSIS (instalação por máquina, requer elevação).
3. Atalho criado no menu Iniciar como **RT Mensor**.

Funciona em **Windows 10/11** (a versão 11 já vem com o WebView2 necessário).

## Atualizações automáticas

O app verifica novas versões ao iniciar e a cada ~4 horas em background.
Quando uma versão nova é publicada aqui, o app:

1. Detecta automaticamente via `latest.json` deste repositório.
2. Avisa o usuário com um banner discreto.
3. Baixa em segundo plano e aplica na próxima reinicialização.

Nenhum servidor externo é envolvido — o updater consulta diretamente
o GitHub. Sem coleta de telemetria, sem login, sem rede além do
download da versão nova.

## Funciona offline

Após instalado, o RT Mensor **não precisa de conexão** para:

- Importar documentos fiscais (XLSX, CSV, PDF)
- Calcular apurações de PIS/COFINS
- Gerar grade fiscal, diagnóstico, oportunidades, relatórios
- Editar planilhas dinâmicas com filtros, ordenação e tabelas dinâmicas
- Exportar tudo em XLSX

Internet só é usada para a checagem de atualização (opcional, pode ser
desligada nas configurações).

## Onde ficam seus dados

| Item                   | Localização                                              |
|------------------------|----------------------------------------------------------|
| Banco principal        | `%APPDATA%\RT Mensor\data\rtm.sqlite`                    |
| Backups automáticos    | `%APPDATA%\RT Mensor\backups\rtm-YYYYMMDD-HHMM.sqlite`   |
| Documentos importados  | `%APPDATA%\RT Mensor\documents\<cliente_id>\…`           |
| Logs                   | `%APPDATA%\RT Mensor\logs\rtm-YYYY-MM-DD.log`            |
| Configuração           | `%APPDATA%\RT Mensor\config.toml`                        |

**Tudo local, em arquivos seus.** Backup é uma simples cópia do
diretório `%APPDATA%\RT Mensor\`.

## Histórico de versões

Veja a aba [Releases](https://github.com/OLuskaD3/RT-Mensor-App-Releases/releases)
para changelog de cada versão.

## Suporte

Suporte oficial via Mênsor & Martins. Para problemas técnicos,
inclua na descrição:

- Versão do app (Configurações → Sobre)
- Sistema operacional e versão
- Arquivo de log do dia em `%APPDATA%\RT Mensor\logs\`

## Sobre a Mênsor & Martins

Site: https://mensormartins.com.br

---

**Este repositório contém apenas os binários publicados.** O código-fonte
do RT Mensor é mantido em repositório separado da organização.
