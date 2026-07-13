---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.apple.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@particle.io"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: particle.io
  spf: true
hosts:
- cert_expires: Sep 25 03:23:43 2026 GMT
  host: www.particle.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: docs.particle.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.particle.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Particle Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Particle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Particle
provider_slug: particle-io
slug: particle-io-domain-security
source_filename: particle-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.particle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.particle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\n- host: api.particle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: particle.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@particle.io\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-io/refs/heads/main/security/particle-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cellular
- Cloud Functions
- Connectivity
- Device Management
- Edge
- Firmware
- Fleet Management
- IoT
- OTA
- Webhooks
- Wi-Fi
---
