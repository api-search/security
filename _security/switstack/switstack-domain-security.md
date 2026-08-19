---
api_specs:
- filename: switstack-switcloud-openapi.yml
  format: yaml
  label: Switcloud API
  slug: switcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-switcloud-openapi.yml
- filename: switstack-swittest-openapi.yml
  format: yaml
  label: Swittest API
  slug: swittest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/openapi/switstack-swittest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: switstack.io
  spf: true
hosts:
- cert_expires: Oct  8 05:17:35 2026 GMT
  host: www.switstack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 13:49:18 2026 GMT
  host: docs.switstack.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: switcloud.switstack.io
  https: false
kind: domain-security
layout: security
method: probed
name: Switstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Switstack, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Switstack
provider_slug: switstack
slug: switstack-domain-security
source_filename: switstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.switstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:17:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.switstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:49:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: switcloud.switstack.io\n  https: false\ndomains:\n- domain: switstack.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/switstack/refs/heads/main/security/switstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech Insurtech
- payments
- emv
- emv-level-2
- card-present
- point-of-sale
- softpos
- tap-to-pay
- payment-terminals
- in-store-payments
- pci-mpoc
- certification-testing
- retail-payments
- estate-management
---
