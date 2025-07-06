# ARQUIVOS FINAIS PROCESSADOS

Este diretório contém todos os arquivos finais criados durante o processamento e padronização dos dados de receitas e preços.

## 📁 CONTEÚDO

### 🍽️ RECEITAS (177 receitas padronizadas)

#### `receitas.txt` (144KB)
- **Formato:** Texto legível para humanos
- **Conteúdo:** 177 receitas completas com dados técnicos
- **Características:**
  - Todas padronizadas para 1kg (1000g total)
  - Ingredientes em gramas
  - Dados técnicos (fator de rendimento, tempo, temperatura)
  - Informações nutricionais por 100g
  - Métodos de preparo e dificuldade
  - Observações técnicas

#### `receitas.json` (234KB)
- **Formato:** JSON estruturado para sistemas
- **Conteúdo:** Mesmas 177 receitas em formato de dados
- **Uso:** Integração com sistemas, APIs, bancos de dados

### 💰 PREÇOS (113 registros de preços)

#### `precos_ingredientes.csv` (13KB)
- **Formato:** CSV para planilhas e sistemas
- **Colunas:** ingrediente, preço_anterior, preço_atual, variação_preço, fornecedor, categoria, data_atualização, data_registro
- **Características:**
  - Dados limpos (sem IDs, emails, campos vazios)
  - Preços formatados em R$
  - Variação percentual calculada
  - Fornecedores com nomes limpos
  - Datas no formato brasileiro (DD/MM/AAAA)

#### `precos_ingredientes.txt` (21KB)
- **Formato:** Texto organizado por categoria
- **Conteúdo:** Histórico de preços legível
- **Organização:** 10 categorias de ingredientes

#### `tabela_precos_padronizada.csv` (4KB)
- **Formato:** CSV de referência
- **Conteúdo:** Lista de ingredientes padronizados por categoria
- **Uso:** Base para consulta de preços e padronização

## 📊 ESTATÍSTICAS

### Receitas:
- **Total:** 177 receitas únicas
- **Originais:** 284 receitas
- **Duplicatas removidas:** 107 receitas
- **Peso padrão:** 1000g cada
- **Dados técnicos:** Completos

### Preços:
- **Total:** 113 registros
- **Categorias:** 10 categorias principais
- **Período:** Março a Junho 2025
- **Fornecedores:** Múltiplos fornecedores

### Categorias de Ingredientes:
- Carnes e Derivados: 37 itens
- Verduras e Hortaliças: 21 itens
- Temperos e Condimentos: 20 itens
- Cereais e Derivados: 17 itens
- Laticínios: 8 itens
- Gorduras e Óleos: 5 itens
- Bebidas: 2 itens
- Açúcares e Adoçantes: 1 item
- Produtos de Limpeza: 1 item
- Pães e Bolos: 1 item

## 🎯 USO RECOMENDADO

### Para Receitas:
1. **receitas.txt** - Leitura, impressão, consulta manual
2. **receitas.json** - Importação em sistemas, apps, APIs

### Para Preços:
1. **precos_ingredientes.csv** - Análise em planilhas, importação em ERP
2. **precos_ingredientes.txt** - Consulta rápida, relatórios
3. **tabela_precos_padronizada.csv** - Referência para novos ingredientes

## 🔄 INTEGRAÇÃO

### Sistema de Custos:
- Use **receitas.json** para ingredientes e quantidades
- Use **precos_ingredientes.csv** para valores atuais
- Calcule custo por receita: Σ(quantidade_ingrediente × preço_unitário)

### Controle de Estoque:
- Use **tabela_precos_padronizada.csv** como base
- Monitore variações com **precos_ingredientes.csv**

## 📅 INFORMAÇÕES TÉCNICAS

- **Processado em:** 06/07/2025
- **Ferramenta:** Claude Code (Anthropic)
- **Formato de datas:** DD/MM/AAAA (brasileiro)
- **Moeda:** Real brasileiro (R$)
- **Encoding:** UTF-8
- **Separador CSV:** Vírgula (,)

---

✅ **Todos os arquivos estão prontos para uso em produção!**