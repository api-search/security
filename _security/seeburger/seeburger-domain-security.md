---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seeburger.com
  spf: true
hosts:
- cert_expires: Dec 16 18:58:50 2026 GMT
  host: www.seeburger.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seeburger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEEBURGER, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SEEBURGER
provider_slug: seeburger
slug: seeburger-domain-security
source_filename: seeburger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seeburger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 18:58:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seeburger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seeburger/refs/heads/main/security/seeburger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Integration
- Cloud
- B2B
- API
---
