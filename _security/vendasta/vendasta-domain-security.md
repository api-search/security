---
api_specs:
- filename: vendasta-marketplace-openapi-original.yml
  format: yaml
  label: Vendasta Marketplace API V1
  slug: vendasta-marketplace-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-marketplace-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vendasta.com
  spf: true
hosts:
- cert_expires: Sep  3 05:38:44 2026 GMT
  host: www.vendasta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:24:26 2026 GMT
  host: developers.vendasta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:24:26 2026 GMT
  host: developers-demo.vendasta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vendasta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vendasta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vendasta
provider_slug: vendasta
slug: vendasta-domain-security
source_filename: vendasta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vendasta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 05:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.vendasta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:24:26 2026 GMT\n  hsts: false\n- host: developers-demo.vendasta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:24:26 2026 GMT\n  hsts: false\ndomains:\n- domain: vendasta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/security/vendasta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Marketplace
- SMB
- White Label
- Reseller
- Marketing
- CRM
- Digital Agency
- Platform
---
