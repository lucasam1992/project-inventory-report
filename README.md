# Boas vindas ao repositório do projeto de Relatório de Estoque!

O projeto teve como intuito o desenvolvimento de um gerador de relatórios que recebe arquivos de entrada (`CSV`, `JSON` e `XML`) referente a dados de um estoque e gera um relatório. Foram praticados os conceitos de programação orientada a objetos. 

## Tecnologias Usadas
- Python

## Rodando o Projeto Localmente

1° `git clone https://github.com/tryber/sd-010-a-inventory-report.git` - Clone o repositório para sua máquina <br />
2° `cd sd-010-a-inventory-report` - Entre na pasta do repositório clonado <br />
3° `python3 -m venv .venv && source .venv/bin/activate` - Crie e ative o ambiente virtual para o projeto <br />
4° `python3 -m pip install -r dev-requirements.txt` - Instale as dependências <br /> 
 

## Requisitos

- 1 - Criar um método `generate` numa classe `SimpleReport` do módulo `inventory_report/reports/simple_report.py`. Esse método deverá receber dados numa lista contendo estruturas do tipo `dict` e deverá retornar uma string formatada como um relatório.

- 2 - Criar um método `generate` numa classe `CompleteReport` do módulo `inventory_report/reports/complete_report.py`. Esse método deverá receber dados numa lista contendo estruturas do tipo `dict` e deverá retornar uma string formatada como um relatório.

- 3 - Criar um método `import_data` dentro de uma classe `Inventory` do módulo `inventory_report/inventory/inventory.py`, capaz de ler um arquivo CSV o qual o caminho é passado como parâmetro.

- 4 - Criar um método `import_data` dentro de uma classe `Inventory` do módulo `inventory_report/inventory/inventory.py`, capaz de ler um arquivo JSON o qual o caminho é passado como parâmetro.

- 5 - Criar um método `import_data` dentro de uma classe `Inventory` do módulo `inventory_report/inventory/inventory.py`, capaz de ler um arquivo XML o qual o caminho é passado como parâmetro.

- 6 - Criar uma classe abstrata `Importer` no módulo `inventory_report/importer/importer.py`, que terá três classes herdeiras: `CsvImporter`, `JsonImporter` e `XmlImporter`, cada uma definida em seu respectivo módulo.

- 7 - Criar uma classe `InventoryIterator` no módulo `inventory_report/inventory/inventory_iterator.py`, que implementa a interface de um iterator (`Iterator`). A classe `InventoryRefactor` deve implementar o método `__iter__`, que retornará este iterador.

- 8 - Requisito Bônus - Não Implementado - Preencha a função `main` no módulo `inventory_report/main.py` que, ao receber pela linha de comando o caminho de um arquivo e o tipo de relatório, devolve o relatório correto.

## Autores

- Bruno Mendes
- Lucas Machado