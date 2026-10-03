---
api_specs:
- filename: bitbank-applications-api-openapi.yml
  format: yaml
  label: bitbank Applications API
  slug: bitbank-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-applications-api-openapi.yml
- filename: bitbank-bitbank-api-api-openapi.yml
  format: yaml
  label: bitbank Bitbank API
  slug: bitbank-bitbank-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-bitbank-api-api-openapi.yml
- filename: bitbank-copilot-install-api-openapi.yml
  format: yaml
  label: bitbank Copilot Install API
  slug: bitbank-copilot-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-copilot-install-api-openapi.yml
- filename: bitbank-octocat-api-openapi.yml
  format: yaml
  label: bitbank Octocat API
  slug: bitbank-octocat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-octocat-api-openapi.yml
- filename: bitbank-organizations-api-openapi.yml
  format: yaml
  label: bitbank Organizations API
  slug: bitbank-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-organizations-api-openapi.yml
- filename: bitbank-orgs-api-openapi.yml
  format: yaml
  label: bitbank Orgs API
  slug: bitbank-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-orgs-api-openapi.yml
- filename: bitbank-path-api-openapi.yml
  format: yaml
  label: bitbank Path API
  slug: bitbank-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/openapi/bitbank-path-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitbank.cc
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: bitbank.cc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bitbank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: bitbank
provider_slug: bitbank
slug: bitbank-domain-security
source_filename: bitbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitbank.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitbank.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbank/refs/heads/main/security/bitbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Japan
- Finance
---
