---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sprinto.com
  spf: true
hosts:
- cert_expires: Oct  8 19:35:32 2026 GMT
  host: sprinto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:35:32 2026 GMT
  host: www.sprinto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprinto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprinto, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sprinto
provider_slug: sprinto
slug: sprinto-domain-security
source_filename: sprinto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sprinto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.sprinto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sprinto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprinto/refs/heads/main/security/sprinto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Security
---
