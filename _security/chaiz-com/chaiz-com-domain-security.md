---
api_specs:
- filename: chaiz-com-openapi.yml
  format: yaml
  label: Chaiz Partner API
  slug: chaiz-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaiz-com/openapi/chaiz-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: chaiz.com
  spf: true
hosts:
- cert_expires: Dec 15 01:30:18 2026 GMT
  host: chaiz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chaiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chaiz
provider_slug: chaiz-com
slug: chaiz-com-domain-security
source_filename: chaiz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaiz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 01:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chaiz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chaiz-com/security/chaiz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketplace
- Automotive
- Extended Warranty
- Digital-First
---
