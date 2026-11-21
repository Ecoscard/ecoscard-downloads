# Downloads oficiais Ecoscard

Pacotes compilados das aplicações Ecoscard para clientes e ambientes autorizados. Cada aplicação é publicada em [Releases](../../releases); este README mostra a versão atual de cada uma.

> Este repositório se chamava `Ecoscard-Dowloads` até 20/11/2026. Os links antigos são redirecionados pelo GitHub, mas use o endereço novo: `https://github.com/Ecoscard/ecoscard-downloads`.

## Aplicações disponíveis

<!-- BEGIN ecoscard-dataprep-multos-privatesmart-config -->
### Ecoscard DataPrep MULTOS PrivateSmart Config

Aplicação web para gerar as configurações DataPrep MULTOS PrivateSmart (RegistryDetail, Template Private, PaymentKeys, ALT/ALR/DAT), os componentes de chaves TDES e os PDFs da cerimônia de chaves.

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-dataprep-multos-privatesmart-config` (antes `EcosDataPrepConfigMultosPrivateSmart`) |
| Versão atual | [20.26.11.20](../../releases/tag/ecoscard-dataprep-multos-privatesmart-config-20.26.11.20) — 20/11/2026 |
| Download | [`ecoscard-dataprep-multos-privatesmart-config-20.26.11.20-win-x64.zip`](../../releases/download/ecoscard-dataprep-multos-privatesmart-config-20.26.11.20/ecoscard-dataprep-multos-privatesmart-config-20.26.11.20-win-x64.zip) |
| SHA-256 | `e00f0e42873092db52e03a4d00c0b98e0e039542074a25999916c052e390bf66` |
| Plataforma | Windows x64, autocontido (não exige .NET instalado) |
| Execução | `start.ps1`, abre em `http://127.0.0.1:5080` |
<!-- END ecoscard-dataprep-multos-privatesmart-config -->

<!-- BEGIN ecoscard-dataprep-batch-worker -->
### Ecoscard DataPrep Batch Worker

Serviço de processamento em lote do DataPrep (Worker Service com HSM PKCS#11/KMIP, RabbitMQ e Serilog).

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-dataprep-batch-worker` (antes `EcosDataPrepNetCore`) |
| Versão atual | [20.26.11.20](../../releases/tag/ecoscard-dataprep-batch-worker-20.26.11.20) — 20/11/2026 |
| Download | [`ecoscard-dataprep-batch-worker-20.26.11.20-win-x64.zip`](../../releases/download/ecoscard-dataprep-batch-worker-20.26.11.20/ecoscard-dataprep-batch-worker-20.26.11.20-win-x64.zip) |
| SHA-256 | `1058417aaaec9b1e4cf9a47c4b86ef5612183d7e2b51fecc3f3b7f2e88d865aa` |
| Plataforma | Windows x64 (self-contained, .NET 10, não exige .NET instalado); Docker `suporte472/ecoscard-dataprep-batch-worker` |
| Execução | serviço Windows (`sc create`, ver notas da release); credenciais por variável de ambiente |
<!-- END ecoscard-dataprep-batch-worker -->

<!-- BEGIN ecoscard-dataprep-client-worker -->
### Ecoscard DataPrep Client

Cliente DataPrep que envia arquivos de embossing à API DataPrep e grava os arquivos de personalização. Roda em modo console (um arquivo) ou worker (monitora uma pasta, também como serviço Windows).

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-dataprep-client-worker` (antes `EcosDataPrep.Client`) |
| Versão atual | [20.26.11.21-r2](../../releases/tag/ecoscard-dataprep-client-worker-20.26.11.21-r2) — 21/11/2026 |
| Download | [`ecoscard-dataprep-client-worker-20.26.11.21-r2-win-x64.zip`](../../releases/download/ecoscard-dataprep-client-worker-20.26.11.21-r2/ecoscard-dataprep-client-worker-20.26.11.21-r2-win-x64.zip) |
| SHA-256 | `7dd98512fa7b870d6388ada434358455d9f5dd6b7017e1267eec9316f3c8f4e9` |
| Plataforma | Windows x64 (self-contained, não exige .NET instalado) |
| Execução | `start-worker.bat` (monitora pasta) ou `start-console.bat` (um arquivo); serviço com `install-windows-service.ps1` |
<!-- END ecoscard-dataprep-client-worker -->

<!-- BEGIN ecoscard-dataprep-configeditor-web -->
### Ecoscard DataPrep ConfigEditor

Editor web das configurações do DataPrep (Bootstrap, ProjectProcessing e projetos da API), com validação, diagrama 3D, prévia de payloads e extração de ALU MULTOS.

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-dataprep-configeditor-web` (antes `EcosDataPrepConfigEditorGitRepo`) |
| Versão atual | [20.26.11.19-r5](../../releases/tag/ecoscard-dataprep-configeditor-web-20.26.11.19-r5) — 19/11/2026 |
| Download | [`ecoscard-dataprep-configeditor-web-20.26.11.19-r5-win-x64.zip`](../../releases/download/ecoscard-dataprep-configeditor-web-20.26.11.19-r5/ecoscard-dataprep-configeditor-web-20.26.11.19-r5-win-x64.zip) |
| SHA-256 | `902cdcd204d80833c4c316b9d749b7d4fc43a6a781c02c3effd3edd1dcb51d55` |
| Plataforma | Windows x64 (self-contained, não exige .NET instalado); Docker `suporte472/ecoscard-dataprep-configeditor-web` |
| Execução | `start.bat`, abre em `http://127.0.0.1:5098` |
<!-- END ecoscard-dataprep-configeditor-web -->

<!-- BEGIN ecoscard-cardanalyzer-emv-desktop -->
### Ecoscard CardAnalyzer EMV

Analisador de cartões EMV: simulador de terminal PC/SC (contato e sem contato), validação de ARQC/ARPC e ODA, scripts de emissor e laudos em PDF e Word.

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-cardanalyzer-emv-desktop` (antes `Ecoscard.EmvCardAnalyzer`) |
| Versão atual | [20.26.11.20](../../releases/tag/ecoscard-cardanalyzer-emv-desktop-20.26.11.20) — 20/11/2026 |
| Download | [`ecoscard-cardanalyzer-emv-desktop-20.26.11.20-win-x64.zip`](../../releases/download/ecoscard-cardanalyzer-emv-desktop-20.26.11.20/ecoscard-cardanalyzer-emv-desktop-20.26.11.20-win-x64.zip) |
| SHA-256 | `1cce99a4a3f2718081f35ad0ca6863826ab9f89a997fe760976c673500885d22` |
| Plataforma | Windows x64 (self-contained, não exige .NET instalado); requer leitora com driver PC/SC |
| Execução | `Ecoscard.CardAnalyzer.Emv.Desktop.exe`; configuração autorizada do laboratório em `Data\config.private.xml` (o pacote não contém IMKs) |
<!-- END ecoscard-cardanalyzer-emv-desktop -->

<!-- BEGIN ecoscard-hsm-gateway-worker -->
### Ecoscard HSM Gateway Worker

Gateway TCP para comandos A1 (validação de criptograma EMV) com PKCS#11 direto no HSM. Roda como serviço Windows ou container Docker (`suporte472/ecoscard-hsm-gateway-worker`).

| Item | Valor |
| --- | --- |
| Nome técnico | `ecoscard-hsm-gateway-worker` (antes `EcosWorkerHSMGateway`) |
| Versão atual | [20.26.11.20-r6](../../releases/tag/ecoscard-hsm-gateway-worker-20.26.11.20-r6) — 20/11/2026 |
| Download | [`ecoscard-hsm-gateway-worker-20.26.11.20-r6-win-x64.zip`](../../releases/download/ecoscard-hsm-gateway-worker-20.26.11.20-r6/ecoscard-hsm-gateway-worker-20.26.11.20-r6-win-x64.zip) |
| SHA-256 | `47a1de9d2b537c85dba87fe3dfbf71888b2bb93f32a007d6a1765e0e08c114a2` |
| Plataforma | Windows x64 (self-contained, não exige .NET instalado) |
| Execução | serviço Windows com `instalar_servico.bat`; configuração em `appsettings.json` (modelo incluso) |
<!-- END ecoscard-hsm-gateway-worker -->

## Como instalar

1. Abra a versão atual da aplicação na tabela acima ou em [Releases](../../releases).
2. Baixe o arquivo ZIP e confira o SHA-256:
   - Windows (PowerShell): `Get-FileHash .\arquivo.zip -Algorithm SHA256`
   - Linux: `sha256sum arquivo.zip`
3. Extraia o conteúdo em uma pasta local.
4. Siga as notas da release para configurar e executar a aplicação.

## Versões

As versões seguem a data do build no formato `YY.YY.M.D`: `20.26.11.19` corresponde a 19/11/2026. Uma segunda publicação no mesmo dia recebe o sufixo `-r2`. Releases a partir de 19/11/2026 usam a tag `<nome-técnico>-<versão>`, por exemplo `ecoscard-dataprep-multos-privatesmart-config-20.26.11.19`. Versões publicadas não são substituídas.

## Suporte

Fale com o suporte Ecoscard informando a aplicação, a versão e o SHA-256 do pacote utilizado.
