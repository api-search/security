---
api_specs:
- filename: aopay-openapi-generated.yml
  format: yaml
  label: AOPAY Technology API
  slug: aopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aopay/refs/heads/main/openapi/_ae-authored/aopay-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aopay.in
  spf: true
hosts:
- cert_expires: Nov 23 09:58:41 2026 GMT
  host: aopay.in
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AOPAY Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AOPAY Technology
provider_slug: aopay
slug: aopay-domain-security
source_filename: aopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aopay.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 09:58:41 2026 GMT\n  hsts: false\ndomains:\n- domain: aopay.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aopay/refs/heads/main/security/aopay-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fintech
- Payments
- Banking
- NBFC
- API
---
