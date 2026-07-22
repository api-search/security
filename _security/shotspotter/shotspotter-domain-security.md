---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soundthinking.com
  spf: true
hosts:
- cert_expires: Oct 15 23:14:14 2026 GMT
  host: www.soundthinking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: docs.soundthinking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shotspotter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShotSpotter (SoundThinking), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ShotSpotter (SoundThinking)
provider_slug: shotspotter
slug: shotspotter-domain-security
source_filename: shotspotter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundthinking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:14:14 2026 GMT\n  hsts: false\n- host: docs.soundthinking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: soundthinking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shotspotter/refs/heads/main/security/shotspotter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Public Safety
- Gunshot Detection
- Law Enforcement
- Weapons Detection
- Acoustic Sensors
- Government
- Security
- Webhooks
---
