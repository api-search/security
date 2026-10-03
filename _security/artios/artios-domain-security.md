---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artios.com
  spf: true
hosts:
- cert_expires: Dec 23 04:54:35 2026 GMT
  host: www.artios.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artios
provider_slug: artios
slug: artios-domain-security
source_filename: artios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 04:54:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: artios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artios/refs/heads/main/security/artios-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pharma
- Oncology
- DDR
- Clinical Stage
- Cambridge
---
