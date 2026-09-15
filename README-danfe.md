# Case Study: Endereço de Entrega na DANFE

**Projeto de adequação fiscal e logística em SAP | Liderança técnica e levantamento de requisitos**

> Status: **Em produção** (implantado em 2026)

## Contexto do problema

Em diversos cenários operacionais, a DANFE (Documento Auxiliar da Nota Fiscal Eletrônica) exibia o endereço cadastral do cliente — vinculado ao CNPJ — mesmo quando o local efetivo de entrega da mercadoria era outro.

**Exemplo prático:** uma empresa compra material para uso em uma obra específica, mas o descarregamento acontece em um endereço diferente da sede cadastrada no CNPJ. A DANFE, no entanto, seguia exibindo apenas o endereço da sede — criando uma divergência entre o documento fiscal e a operação real de entrega.

Esse gap foi identificado como um item crítico de auditoria, exigindo uma correção com **urgência de contingência**, dentro do que inicialmente era um projeto de maior escopo.

## Meu papel no projeto

- **Liderei o projeto** do início até a implantação em produção.
- Conduzi o **levantamento de requisitos** diretamente com a área de Coprodutos, mapeando o processo operacional real de expedição e identificando onde a informação do endereço de entrega deveria ser capturada.
- Priorizei o escopo para entregar uma solução de contingência rápida e funcional diante da urgência do item de auditoria, mesmo com o projeto original sendo mais amplo.
- Acompanhei o desenvolvimento em SAP e a validação funcional até a homologação e o go-live.

## Objetivo

Garantir maior aderência aos requisitos de auditoria, rastreabilidade e conformidade fiscal, permitindo a identificação do endereço real de entrega da carga através de informações complementares registradas na emissão da Nota Fiscal.

## Escopo da solução

- Desenvolvimento realizado integralmente no SAP.
- Inclusão do endereço efetivo de entrega durante o processo de expedição.
- Disponibilização das informações de entrega em campos adicionais da DANFE.
- Adequação do processo para que a documentação fiscal reflita corretamente o local de descarga da mercadoria.
- Suporte aos processos de Coprodutos e demais operações que exigem entrega em local diferente do endereço cadastrado no CNPJ do cliente.

## Fluxo do processo

1. **Criação do Pedido/Contrato**
   - O processo inicia com a criação do contrato de venda do material no SAP.
   - Em determinados cenários, o endereço real de descarga é diferente do endereço cadastrado no CNPJ do cliente.

2. **Informação do endereço de entrega**
   - Durante o processo operacional, o endereço efetivo de entrega é informado no SAP em campos de texto utilizados pelo processo logístico e fiscal, incluído no texto do item do contrato, para que a informação seja carregada ao longo de todo o fluxo.

3. **Criação da remessa**
   - A partir do contrato/pedido é criada a remessa de expedição.
   - A informação do endereço de entrega acompanha o item da remessa durante o processamento logístico.

4. **Geração da Nota Fiscal**
   - No momento da emissão da NF, o sistema recupera o endereço de entrega informado anteriormente.
   - O endereço fiscal do cliente continua vinculado ao CNPJ, porém o endereço real de descarga passa a ser disponibilizado em informações complementares da documentação fiscal.

5. **Impressão da DANFE**
   - O endereço real de entrega é apresentado nos Dados Adicionais da DANFE.
   - Transportadores, operadores logísticos e auditores conseguem visualizar o local efetivo da entrega, mesmo quando diferente do endereço cadastral do cliente.

## Benefícios entregues

- Maior conformidade com auditorias internas e externas.
- Redução de divergências entre o endereço fiscal do cliente e o endereço real da operação.
- Melhor rastreabilidade logística das entregas.
- Aumento da confiabilidade das informações utilizadas por áreas operacionais, fiscais e de transporte.

## Tecnologias e processos envolvidos

- SAP SD (Sales and Distribution)
- Emissão de Nota Fiscal Eletrônica (NF-e)
- DANFE
- Processos de Expedição e Logística de Coprodutos

## Resumo executivo

Projeto SAP que possibilita identificar o endereço real de entrega da mercadoria na DANFE por meio de informações complementares, eliminando a dependência exclusiva do endereço vinculado ao CNPJ do cliente e aumentando a rastreabilidade e conformidade do processo fiscal e logístico.

---

*Nota: por questões de confidencialidade, este case study não inclui capturas de tela do sistema, dados de clientes ou configurações internas do SAP. O conteúdo descreve o problema de negócio, minha atuação e o resultado entregue.*
