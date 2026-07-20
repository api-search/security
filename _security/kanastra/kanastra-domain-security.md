---
api_specs:
- filename: kanastra-banking-openapi.yml
  format: yaml
  label: Kanastra Banking API
  slug: kanastra-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/openapi/kanastra-banking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kanastra.com.br
  spf: true
hosts:
- cert_expires: Aug 23 07:22:05 2026 GMT
  host: kanastra.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 12:02:09 2026 GMT
  host: banking.kanastra.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 12:27:51 2026 GMT
  host: banking-sandbox.kanastra.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kanastra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanastra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kanastra
provider_slug: kanastra
slug: kanastra-domain-security
source_filename: kanastra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kanastra.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:22:05 2026 GMT\n  hsts: null\n- host: banking.kanastra.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:02:09 2026 GMT\n  hsts: null\n- host: banking-sandbox.kanastra.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:27:51 2026 GMT\n  hsts: null\ndomains:\n- domain: kanastra.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanastra/refs/heads/main/security/kanastra-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Banking
- Banking as a Service
- Payments
- PIX
- Boleto
- Private Credit
- Fintech
- Brazil
- Wealth Management
---
