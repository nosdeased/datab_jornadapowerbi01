# datab_jornadapowerbi01
Repositório criado para Jornada Power BI Dia 2
![image](https://user-images.githubusercontent.com/63180950/216348379-75d0c3e3-21af-4640-941a-2f1e6b5c521f.png)



Tratamento dos dados:
Converter códigos dos grupos em seus respectivos  nomes : 1:Atacado, 2:Atacarejo, 3:Varejo, 4:Distribuidor
= Table.AddColumn(#"Linhas Classificadas1", "Personalizar", each if [Grupo Cliente] = 1 then "Atacado" else if [Grupo Cliente] = 4 then "Distribuidor" else if [Grupo Cliente] = 2 then "Atacarejo" else if [Grupo Cliente] = 3 then "Varejo" else null, type text)

Nome Medida :
Lucro = SUM(Pedidos[Valor Total]) - SUM(Pedidos[Custo Total])
Margem de Lucro = Margem de Lucro = [Lucro] / SUM(Pedidos[Valor Total])

Botão Clean :
Adicionado

Link:

https://app.powerbi.com/view?r=eyJrIjoiODQ4ZGFmYWYtYjU5ZS00ZWQyLWFiM2UtMGE3OWIzNzVlNjNkIiwidCI6IjY2ZTdiNDNhLWE3ODEtNDc3ZC1iZjJlLTdkZWFmYmQ1NDc3MiJ9
