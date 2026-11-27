---
api_specs:
- filename: factori-ai-people-api-openapi.yml
  format: yaml
  label: Factori People API
  slug: factori-ai-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factori-ai/openapi/factori-ai-people-api-openapi.yml
- filename: factori-ai-poi-api-openapi.yml
  format: yaml
  label: Factori Poi API
  slug: factori-ai-poi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factori-ai/openapi/factori-ai-poi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: factori.ai
  spf: true
hosts:
- cert_expires: Jan 21 06:39:26 2027 GMT
  host: factori.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Factori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factori, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Factori
provider_slug: factori-ai
slug: factori-ai-domain-security
source_filename: factori-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factori.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 06:39:26 2027 GMT\n  hsts: false\ndomains:\n- domain: factori.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/factori-ai/security/factori-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Real-World Data
- Forecasting
- Enterprise
- Analytics
---
