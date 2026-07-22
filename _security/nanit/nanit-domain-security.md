---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@nanit.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nanit.com
  spf: true
hosts:
- cert_expires: Sep 10 16:21:32 2026 GMT
  host: www.nanit.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nanit
provider_slug: nanit
slug: nanit-domain-security
source_filename: nanit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nanit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: nanit.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@nanit.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanit/refs/heads/main/security/nanit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Baby Monitor
- Smart Home
- IoT
- Sleep Tracking
- Connected Devices
- Computer Vision
- Parenting
---
