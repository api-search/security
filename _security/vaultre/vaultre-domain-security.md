---
api_specs:
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE API
  slug: vaultre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-api-v1-3-openapi.yml
  format: yaml
  label: VaultRE Integrator API
  slug: vaultre-integrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-api-v1-3-openapi.yml
- filename: vaultre-aggregator-api-v1-0-openapi.yml
  format: yaml
  label: VaultRE Aggregator API
  slug: vaultre-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/openapi/vaultre-aggregator-api-v1-0-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mrisoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vaultre.com.au
  spf: true
hosts:
- cert_expires: Sep 22 03:07:29 2026 GMT
  host: www.mrisoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: docs.api.vaultre.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: ap-southeast-2.api.vaultre.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vaultre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VaultRE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VaultRE
provider_slug: vaultre
slug: vaultre-domain-security
source_filename: vaultre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mrisoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.vaultre.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: ap-southeast-2.api.vaultre.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mrisoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vaultre.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaultre/refs/heads/main/security/vaultre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Australia
- New Zealand
- PropTech
- CRM
- Property Listings
- Property Management
- Rentals
- Commercial Real Estate
- Webhooks
---
