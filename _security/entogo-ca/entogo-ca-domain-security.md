---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: entogo.ca
  spf: true
hosts:
- cert_expires: Dec 22 21:00:26 2026 GMT
  host: entogo.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entogo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Entogo
provider_slug: entogo-ca
slug: entogo-ca-domain-security
source_filename: entogo-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entogo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:00:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: entogo.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/entogo-ca/security/entogo-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Cleantech
- Transformers
- Switchgear
---
