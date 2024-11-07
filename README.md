
# Tradutor de Textos e Documentos com Azure AI

## Descrição
Este projeto é uma ferramenta de tradução que utiliza os serviços Azure Cognitive Services e Azure OpenAI para traduzir textos, documentos Word e conteúdo de páginas web. O sistema suporta múltiplos idiomas e oferece diferentes métodos de tradução.

## Funcionalidades
- Tradução de texto simples
- Tradução de documentos Word (.docx)
- Extração e tradução de conteúdo de páginas web
- Integração com Azure OpenAI para traduções mais contextualizadas

## Pré-requisitos
Instale as dependências necessárias:
```bash
pip install beautifulsoup4 openai langchain-openai requests python-docx
```

## Configuração
Configure suas credenciais Azure:
- Subscription Key do Azure Translator
- Endpoint do Azure Translator
- Localização do serviço
- Credenciais do Azure OpenAI

Substitua as seguintes variáveis no código:
- `YOUR_SUBSCRIPTION_KEY`
- `YOUR_LOCATION`
- `YOUR_ENDPOINT`
- `YOUR_API_KEY`
- `YOUR_API_VERSION`
- `YOUR_DEPLOYMENT_NAME`

## Uso

### Tradução de Texto Simples
```python
translated_text = translate_text("Hello World", "pt-br")
```

### Tradução de Documento Word
```python
translated_doc_path = translate_document("caminho/do/documento.docx")
```

### Extração de Texto de URL
```python
text = extract_text_from_url("https://exemplo.com")
```

### Tradução com Azure OpenAI
```python
translated_article = translate_article("texto para traduzir", "português")
```

## Estrutura do Projeto
- `translate_text()`: Função para tradução de texto simples
- `translate_document()`: Função para tradução de documentos Word
- `extract_text_from_url()`: Função para extração de texto de URLs
- `translate_article()`: Função para tradução usando Azure OpenAI


## Limitações
- Necessita de credenciais válidas do Azure
- Sujeito aos limites de requisições dos serviços Azure
- Requer conexão com internet


