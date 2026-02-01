# 🔀 SAP-Process-Integration-Runtime
## SAP BTP CPI - SAP Process Integration Runtime


Este repositório demonstra como o SAP Process Integration Runtime é o componente essencial que torna as integrações do SAP Integration Suite realmente operacionais.
Ele garante que os iFlows sejam executados com segurança, desempenho e confiabilidade, conectando diferentes sistemas dentro e fora do ecossistema SAP.

Para qualquer cenário de integração no SAP BTP, entender o funcionamento do Runtime é fundamental para arquiteturas robustas e escaláveis.

![Capa](imagens/capa-linkedin.png)


## O que é o SAP Process Integration Runtime?

O SAP Process Integration Runtime é o motor de execução dos cenários de integração criados no Cloud Integration (CPI).
Tudo o que você modela no iFlow só funciona em produção porque o Process Integration Runtime executa essas integrações.

### Ele é responsável por:

* Processar mensagens

* Orquestrar fluxos

* Aplicar transformações

* Gerenciar conectividade

* Garantir segurança e monitoramento

* Onde o Process Integration Runtime atua?

* Ele atua após a modelagem do iFlow, no momento em que a integração entra em execução.

### Fluxo simplificado:

* O iFlow é modelado no Cloud Integration

* O iFlow é deployado

* O Process Integration Runtime executa o fluxo

* As mensagens são processadas entre sistemas

### Principais responsabilidades do Process Integration Runtime
1. Execução dos iFlows

* Processa mensagens síncronas e assíncronas

* Controla etapas como roteamento, mapeamento e validação

2. Orquestração de Integrações

* Define a sequência de chamadas

* Gerencia paralelismo e condições

* Controla exceções e erros

3. Conectividade

* Suporta diversos adaptadores:

* HTTP / HTTPS

* OData

* SOAP

* SFTP

* IDoc

* RFC

* SuccessFactors, Ariba, etc.

4. Segurança

* Autenticação (OAuth2, Basic, Client Certificate)

* Criptografia

* Armazenamento seguro de credenciais

* Integração com Keystore e Credential Store

5. Monitoramento e Logging

* Monitoramento de mensagens

* Logs técnicos e funcionais

* Reprocessamento de mensagens com erro

* Métricas de performance


## 📦 Exemplo prático – Como utilizar para um cenário de Demonstração como confiurar é utilizar. (Não recomendado em Produção)




---

## 📥 Exemplo de Payload JSON

O JSON utilizado no teste pode ser encontrado em:

📄 [`json/ordens.json`](json/ordens.json)

```json
{
  "Orders": {
    "Pedidos": [
      { "id": 1, "value": 100 },
      { "id": 2, "value": 200 },
      { "id": 3, "value": 300 }
    ]
  }
}
```

## 🔄 Fluxo do iFlow

![Fluxo](imagens/Screenshot_1.png)
![Fluxo](imagens/Screenshot_2.png)
![Fluxo](imagens/Screenshot_3.png)
![Fluxo](imagens/Screenshot_4.png)
![Fluxo](imagens/Screenshot_5.png)
![Fluxo](imagens/Screenshot_6.png)
![Fluxo](imagens/Screenshot_7.png)
![Fluxo](imagens/Screenshot_8.png)
![Fluxo](imagens/Screenshot_9.png)
![Fluxo](imagens/Screenshot_10.png)
![Fluxo](imagens/Screenshot_11.png)


## 📦 Exemplo prático – iFlow para baixar

📦 [Download do iFlow – SPLITTER.zip](Package/SPLITTER.zip)

> O arquivo pode ser importado diretamente no SAP Integration Suite (CPI).
