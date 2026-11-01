---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: harper.insure
  spf: false
hosts:
- cert_expires: Dec 31 09:21:46 2026 GMT
  host: www.harper.insure
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Harper Insure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Harper
provider_slug: harper-insure
slug: harper-insure-domain-security
source_filename: harper-insure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harper.insure\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 09:21:46 2026 GMT\n  hsts: false\ndomains:\n- domain: harper.insure\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/harper-insure/security/harper-insure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- InsurTech
- API
- Digital
---
