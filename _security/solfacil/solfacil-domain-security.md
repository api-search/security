---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: solfacil.com.br
  spf: true
hosts:
- cert_expires: Sep 14 03:50:05 2026 GMT
  host: landing.solfacil.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solfacil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solfacil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Solfacil
provider_slug: solfacil
slug: solfacil-domain-security
source_filename: solfacil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landing.solfacil.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:50:05 2026 GMT\n  hsts: false\ndomains:\n- domain: solfacil.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solfacil/refs/heads/main/security/solfacil-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Clean Energy
- Solar Energy
- Fintech
- Financing
- Energy Storage
- Distributor
- Brazil
---
