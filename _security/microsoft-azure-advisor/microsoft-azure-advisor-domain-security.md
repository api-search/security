---
api_specs:
- filename: microsoft-azure-advisor-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Operations API
  slug: microsoft-azure-advisor-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-operations-api-openapi.yml
- filename: microsoft-azure-advisor-recommendations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Recommendations API
  slug: microsoft-azure-advisor-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-recommendations-api-openapi.yml
- filename: microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Advisor Score Entities API
  slug: microsoft-azure-advisor-advisorscoreentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-advisorscoreentities-api-openapi.yml
- filename: microsoft-azure-advisor-metadataentities-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Metadata Entities API
  slug: microsoft-azure-advisor-metadataentities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-metadataentities-api-openapi.yml
- filename: microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resiliency Reviews API
  slug: microsoft-azure-advisor-resiliencyreviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resiliencyreviews-api-openapi.yml
- filename: microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Resource Recommendation Bases API
  slug: microsoft-azure-advisor-resourcerecommendationbases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-resourcerecommendationbases-api-openapi.yml
- filename: microsoft-azure-advisor-subscriptions-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Subscriptions API
  slug: microsoft-azure-advisor-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-subscriptions-api-openapi.yml
- filename: microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
  format: yaml
  label: Microsoft Azure Advisor Suppression Contracts API
  slug: microsoft-azure-advisor-suppressioncontracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-advisor/openapi/microsoft-azure-advisor-suppressioncontracts-api-openapi.yml
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
- cert_expires: Jan 30 14:50:49 2027 GMT
  host: microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Azure Advisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Advisor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Advisor
provider_slug: microsoft-azure-advisor
slug: microsoft-azure-advisor-domain-security
source_filename: microsoft-azure-advisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 14:50:49 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-advisor/security/microsoft-azure-advisor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advisor
- Best Practices
- Cost Optimization
- Microsoft Azure
- Optimization
- Recommendations
---
