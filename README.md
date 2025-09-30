# Agregador de Dados para Imposto de Renda (Excel)

> Projeto de Organização e Agregação de Dados para Declaração de IR.  
> Ferramenta em Excel para centralizar informações financeiras, organizar lançamentos e gerar relatórios de apoio à declaração anual.

---

## Visão Geral
Esta planilha foi construída com o objetivo de **organizar dados essenciais para o Imposto de Renda Pessoa Física (IRPF)**.  
Ela ajuda o usuário a manter controle eficiente de:
- Rendimentos (salários, honorários, aluguéis, dividendos, etc.);
- Despesas dedutíveis (saúde, educação, previdência, etc.);
- Bens e direitos (imóveis, veículos, aplicações financeiras);
- Dívidas e ônus;
- Informações de apoio (ex.: CNPJs de fontes pagadoras, número de processos, etc.).

A ferramenta inclui menus de navegação, validações automáticas, tabelas estruturadas e links rápidos para facilitar o uso.

---

## Funcionalidades Principais
- **Menu de Navegação** para acesso rápido às seções da planilha;
- **Validações automáticas** (listas suspensas, bloqueio de células não editáveis, alertas);
- **Campos pré-formatados** para CPF, CNPJ e datas;
- **Links rápidos** para páginas de referência (Receita Federal, bancos, corretoras);
- **Relatórios Resumo** (visão consolidada de rendimentos, deduções e patrimônio).

---

## Exemplos de Recursos no Excel
- **Validação de Dados (lista suspensa):**  
  Menu suspenso para selecionar tipo de rendimento (Salário, Dividendos, Aluguéis, Outros).  
  ```excel
  Dados > Validação de Dados > Lista
  Fonte: Salário;Dividendos;Aluguéis;Outros

Cálculo de totais:
=SOMA(Tabela_Rendimentos[Valor])

Classificação automática de CPF/CNPJ:
Usar máscara com formatação personalizada 000\.000\.000\-00 ou 00\.000\.000/0000\-00.

Links rápidos (hiperlink):
=HIPERLINK("https://www.gov.br/receitafederal", "Receita Federal")

Relatórios disponíveis
Resumo de Rendimentos (consolidado por fonte pagadora);
Resumo de Despesas Dedutíveis (total por categoria);
Resumo de Bens e Direitos (comparação ano-base atual vs. anterior);
Resumo Consolidado (visão geral do que será informado na declaração).

Como usar
Abra a planilha Agregador_ImpostoRenda.xlsx;
Use o menu inicial para navegar entre seções;
Preencha os campos de acordo com os comprovantes fornecidos (rendimentos, despesas, etc.);
Acompanhe os totais automáticos e relatórios de resumo;
Utilize os links rápidos para acessar a Receita Federal e outras fontes oficiais.
