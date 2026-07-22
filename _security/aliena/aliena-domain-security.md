---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aliena.sg
  spf: true
hosts:
- cert_expires: Sep  2 06:56:07 2026 GMT
  host: aliena.sg
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aliena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aliena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aliena
provider_slug: aliena
slug: aliena-domain-security
source_filename: aliena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aliena.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:56:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: aliena.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aliena/refs/heads/main/security/aliena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Satellites
- Electric Propulsion
- Aerospace
- Hardware
- Deep Tech
- Singapore
---
