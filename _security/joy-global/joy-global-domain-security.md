---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mining.komatsu
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: mining.komatsu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joy Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joy Global (Komatsu Mining), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Joy Global (Komatsu Mining)
provider_slug: joy-global
slug: joy-global-domain-security
source_filename: joy-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mining.komatsu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mining.komatsu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joy-global/refs/heads/main/security/joy-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mining
- Heavy Equipment
- Industrial
---
