---
api_specs:
- filename: ecocheck-ai-about-api-openapi.yml
  format: yaml
  label: EcoCheck About API
  slug: ecocheck-ai-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-about-api-openapi.yml
- filename: ecocheck-ai-articles-api-openapi.yml
  format: yaml
  label: EcoCheck Articles API
  slug: ecocheck-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-articles-api-openapi.yml
- filename: ecocheck-ai-cbam-api-openapi.yml
  format: yaml
  label: EcoCheck Cbam API
  slug: ecocheck-ai-cbam-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-cbam-api-openapi.yml
- filename: ecocheck-ai-health-api-openapi.yml
  format: yaml
  label: EcoCheck Health API
  slug: ecocheck-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-health-api-openapi.yml
- filename: ecocheck-ai-obligation-api-openapi.yml
  format: yaml
  label: EcoCheck Obligation API
  slug: ecocheck-ai-obligation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-obligation-api-openapi.yml
- filename: ecocheck-ai-pricing-api-openapi.yml
  format: yaml
  label: EcoCheck Pricing API
  slug: ecocheck-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-pricing-api-openapi.yml
- filename: ecocheck-ai-regulations-api-openapi.yml
  format: yaml
  label: EcoCheck Regulations API
  slug: ecocheck-ai-regulations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-regulations-api-openapi.yml
- filename: ecocheck-ai-search-api-openapi.yml
  format: yaml
  label: EcoCheck Search API
  slug: ecocheck-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-search-api-openapi.yml
- filename: ecocheck-ai-services-api-openapi.yml
  format: yaml
  label: EcoCheck Services API
  slug: ecocheck-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecocheck-ai/openapi/ecocheck-ai-services-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ecocheck.ai
  spf: true
hosts:
- cert_expires: Jan  3 12:16:27 2027 GMT
  host: ecocheck.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EcoCheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: EcoCheck
provider_slug: ecocheck-ai
slug: ecocheck-ai-domain-security
source_filename: ecocheck-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecocheck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:16:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ecocheck.ai\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecocheck-ai/security/ecocheck-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Greenhouse Gas
- Emissions
- Vietnam
- Software-as-a-Service
- Climate
---
