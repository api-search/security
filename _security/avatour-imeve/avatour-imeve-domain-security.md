---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avatour.co
  spf: true
hosts:
- cert_expires: Sep 16 14:48:32 2026 GMT
  host: avatour.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avatour Imeve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVATOUR, Imeve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AVATOUR, Imeve
provider_slug: avatour-imeve
slug: avatour-imeve-domain-security
source_filename: avatour-imeve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avatour.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avatour.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avatour-imeve/refs/heads/main/security/avatour-imeve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Collaboration
- 360 Video
- Remote Work
- Telepresence
- Inspection
- Virtual Tours
---
