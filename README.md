# NotaFácil

O **NotaFácil** é um sistema inteligente e 100% executado no navegador (sem necessidade de backend) para leitura de PDFs de Notas Fiscais (Danfe), fragmentação de itens por unidade e geração de relatórios de rateio.

## Como funciona?

1. **Upload da Nota**: Você faz o upload do arquivo PDF da sua Danfe.
2. **Processamento Inteligente**: O sistema extrai automaticamente o nome da Empresa Emissora, Destinatário, Número da NF, e processa os itens da nota.
3. **Fragmentação de Itens**: Se um item possuir quantidade maior que 1 (ex: 3 Cabos de Rede), o sistema irá separar esse item em 3 linhas diferentes. Isso permite que você aplique **Chamados** e **Rateios** diferentes para cada unidade do mesmo produto.
4. **Preenchimento e Exportação**: Você preenche o chamado, o setor do rateio e observações, e com um clique gera um PDF final lindamente formatado!

## Exemplo de Uso

1. Abra o `index.html` (ou acesse o link hospedado).
2. Selecione a nota fiscal `Danfe_Exemplo.pdf` (Exemplo: 5 Cabos USB, Valor Unitário R$20).
3. A tabela gerada terá 5 linhas de "Cabo USB", cada uma com Quantidade 1 e Valor Total R$20.
4. Na linha 1, você insere o Rateio "Depto de TI". Na linha 2, "Depto de Marketing", e assim por diante.
5. Clique em **Gerar PDF de Rateio** e salve seu relatório preenchido e formatado!

## Funcionalidades

- **Extração via OCR/PDF.js**: Identificação de linhas através de agrupamento com tolerância Y.
- **PWA (Progressive Web App)**: Pode ser instalado no seu computador ou celular como um aplicativo nativo.
- **Totalmente Offline**: Após carregado a primeira vez, o processamento ocorre no seu computador, mantendo seus dados fiscais 100% seguros e privados.

Desenvolvido por **Dan Martins**.
