# Scraping de Agências dos Correios
## Este repositório contém um script de web scraping para coletar informações de agências dos Correios. O código foi desenvolvido para extrair e organizar dados de endereços, como nome da agência, logradouro, número, CEP, e informações de localização (latitude e longitude).

### Funcionalidades
Web Scraping dos Correios: Coleta dados de agências dos Correios, incluindo nome, endereço, número, CEP, e link do Google Maps.
Listas de Estabelecimentos Comerciais e Organizações: Contém listas de estabelecimentos comerciais e organizações selecionadas para a extração de endereços.

### Estrutura do Código
Função principal (main): Realiza o scraping de todos os estados e processa as agências dos Correios.
Funções auxiliares:
init_spark_session: Inicializa a sessão Spark.
init_webdriver: Inicializa o WebDriver do Chrome.
get_select_options_by_value: Obtém as opções de um elemento select na página.
extract_agency_data: Extrai os dados de uma agência.
save_data_to_csv: Converte os dados extraídos para um DataFrame do Spark e salva em um arquivo CSV.

### Como Usar
1º - Instale as dependências: pip install pyspark selenium
2º - Defina o diretório onde os arquivos serão salvos na penúltima célula
3º - Execute o script completo

O script coletará os dados dos Correios, organizando-os e salvando-os em um arquivo CSV dentro do diretório determinado.
