---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rollins.com
  spf: true
hosts:
- cert_expires: Oct  5 12:04:54 2026 GMT
  host: www.rollins.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.rollins.com
  https: false
- host: api.rollins.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rollins Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rollins, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rollins
provider_slug: rollins
slug: rollins-domain-security
source_filename: rollins-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rollins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:04:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rollins.com\n  https: false\n- host: api.rollins.com\n  https: false\ndomains:\n- domain: rollins.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rollins/refs/heads/main/security/rollins-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pest Control
- Services
---
