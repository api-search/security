---
api_specs:
- filename: ofx-aisp-openapi-generated.yml
  format: yaml
  label: OFX AISP API
  slug: aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-aisp-openapi-generated.yml
- filename: ofx-ncp-openapi-generated.yml
  format: yaml
  label: OFX NCP API
  slug: ncp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-ncp-openapi-generated.yml
- filename: ofx-pisp-openapi-generated.yml
  format: yaml
  label: OFX PISP API
  slug: pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-pisp-openapi-generated.yml
- filename: ofx-rates-openapi-generated.yml
  format: yaml
  label: OFX Rates API
  slug: rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/openapi/_ae-authored/ofx-rates-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ofx.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.ofx.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 09:16:12 2026 GMT
  host: api-docs.ofx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: beta.api.ofx.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ofx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OFX, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OFX
provider_slug: ofx
slug: ofx-domain-security
source_filename: ofx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ofx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api-docs.ofx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 09:16:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: beta.api.ofx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ofx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofx/refs/heads/main/security/ofx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Money Transfer
- Fintech
- Banking
---
