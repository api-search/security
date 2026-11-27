---
api_specs:
- filename: ohmyfin-ai-companysearch-api-openapi.yml
  format: yaml
  label: Ohmyfin Company Search API
  slug: ohmyfin-ai-companysearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohmyfin-ai/openapi/ohmyfin-ai-companysearch-api-openapi.yml
- filename: ohmyfin-ai-reference-api-openapi.yml
  format: yaml
  label: Ohmyfin Reference API
  slug: ohmyfin-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohmyfin-ai/openapi/ohmyfin-ai-reference-api-openapi.yml
- filename: ohmyfin-ai-sanctions-api-openapi.yml
  format: yaml
  label: Ohmyfin Sanctions API
  slug: ohmyfin-ai-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohmyfin-ai/openapi/ohmyfin-ai-sanctions-api-openapi.yml
- filename: ohmyfin-ai-tradecheck-api-openapi.yml
  format: yaml
  label: Ohmyfin Trade Check API
  slug: ohmyfin-ai-tradecheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohmyfin-ai/openapi/ohmyfin-ai-tradecheck-api-openapi.yml
- filename: ohmyfin-ai-treasury-api-openapi.yml
  format: yaml
  label: Ohmyfin Treasury API
  slug: ohmyfin-ai-treasury-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohmyfin-ai/openapi/ohmyfin-ai-treasury-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@ohmyfin.ai"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ohmyfin.ai
  spf: true
hosts:
- cert_expires: Feb  1 16:47:06 2027 GMT
  host: ohmyfin.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ohmyfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ohmyfin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ohmyfin
provider_slug: ohmyfin-ai
slug: ohmyfin-ai-domain-security
source_filename: ohmyfin-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohmyfin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 16:47:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ohmyfin.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@ohmyfin.ai\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ohmyfin-ai/security/ohmyfin-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Treasury
- Cross-Border Payments
- Sanctions Screening
- Correspondent Banking
- Financial Institutions
---
