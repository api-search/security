---
api_specs:
- filename: azure-document-intelligence-custom-api-openapi.yml
  format: yaml
  label: Azure AI Document Intelligence Custom API
  slug: azure-document-intelligence-custom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-document-intelligence/openapi/azure-document-intelligence-custom-api-openapi.yml
- filename: azure-document-intelligence-layout-api-openapi.yml
  format: yaml
  label: Azure AI Document Intelligence Layout API
  slug: azure-document-intelligence-layout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-document-intelligence/openapi/azure-document-intelligence-layout-api-openapi.yml
- filename: azure-document-intelligence-prebuilt-api-openapi.yml
  format: yaml
  label: Azure AI Document Intelligence Prebuilt API
  slug: azure-document-intelligence-prebuilt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-document-intelligence/openapi/azure-document-intelligence-prebuilt-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <your-resource>.cognitiveservices.azure.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure AI Document Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure AI Document Intelligence, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure AI Document Intelligence
provider_slug: azure-document-intelligence
slug: azure-document-intelligence-domain-security
source_filename: azure-document-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <your-resource>.cognitiveservices.azure.com\n  https: false\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-document-intelligence/security/azure-document-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Document AI
- Microsoft Azure
- Intelligent Document Processing
- OCR
- Microsoft
- REST
---
