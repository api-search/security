---
api_specs:
- filename: evidujzdarma-cz-account-api-openapi.yml
  format: yaml
  label: EvidujZdarma Account API
  slug: evidujzdarma-cz-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-account-api-openapi.yml
- filename: evidujzdarma-cz-closings-api-openapi.yml
  format: yaml
  label: EvidujZdarma Closings API
  slug: evidujzdarma-cz-closings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-closings-api-openapi.yml
- filename: evidujzdarma-cz-oauth-api-openapi.yml
  format: yaml
  label: EvidujZdarma OAuth API
  slug: evidujzdarma-cz-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-oauth-api-openapi.yml
- filename: evidujzdarma-cz-sales-api-openapi.yml
  format: yaml
  label: EvidujZdarma Sales API
  slug: evidujzdarma-cz-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-sales-api-openapi.yml
- filename: evidujzdarma-cz-units-api-openapi.yml
  format: yaml
  label: EvidujZdarma Units API
  slug: evidujzdarma-cz-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-units-api-openapi.yml
- filename: evidujzdarma-cz-webhooks-api-openapi.yml
  format: yaml
  label: EvidujZdarma Webhooks API
  slug: evidujzdarma-cz-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: evidujzdarma.cz
  spf: true
hosts:
- cert_expires: Dec 31 16:20:59 2026 GMT
  host: evidujzdarma.cz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EvidujZdarma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EvidujZdarma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: EvidujZdarma
provider_slug: evidujzdarma-cz
slug: evidujzdarma-cz-domain-security
source_filename: evidujzdarma-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evidujzdarma.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:20:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: evidujzdarma.cz\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/evidujzdarma-cz/security/evidujzdarma-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Czech Republic
- EET
---
