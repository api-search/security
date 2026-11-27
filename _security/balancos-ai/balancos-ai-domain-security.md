---
api_specs:
- filename: balancos-ai-bcb-api-openapi.yml
  format: yaml
  label: Balanços.AI BCB API
  slug: balancos-ai-bcb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-bcb-api-openapi.yml
- filename: balancos-ai-cvm-api-openapi.yml
  format: yaml
  label: Balanços.AI CVM API
  slug: balancos-ai-cvm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-cvm-api-openapi.yml
- filename: balancos-ai-empresas-api-openapi.yml
  format: yaml
  label: Balanços.AI Empresas API
  slug: balancos-ai-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/balancos-ai/openapi/balancos-ai-empresas-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: balancos.ai
  spf: true
hosts:
- cert_expires: Jan  7 07:06:30 2027 GMT
  host: balancos.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Balanços.AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balanços.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Balanços.AI
provider_slug: balancos-ai
slug: balancos-ai-domain-security
source_filename: balancos-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balancos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:06:30 2027 GMT\n  hsts: false\ndomains:\n- domain: balancos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/balancos-ai/security/balancos-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Brazil
- Public Data
- Financial Statements
---
