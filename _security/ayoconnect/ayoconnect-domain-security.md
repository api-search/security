---
api_specs:
- filename: ayoconnect-bill-api-openapi.yml
  format: yaml
  label: Ayoconnect Bill API
  slug: ayoconnect-bill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ayoconnect/openapi/ayoconnect-bill-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ayoconnect.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ayopop.id
  spf: true
hosts:
- cert_expires: Dec 13 01:54:29 2026 GMT
  host: www.ayoconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: dev0.openapi.ayopop.id
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ayoconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ayoconnect, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ayoconnect
provider_slug: ayoconnect
slug: ayoconnect-domain-security
source_filename: ayoconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ayoconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev0.openapi.ayopop.id\n  https: false\ndomains:\n- domain: ayoconnect.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: ayopop.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ayoconnect/security/ayoconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Indonesia
---
