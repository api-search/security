---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: buildots.com
  spf: true
hosts:
- cert_expires: Aug 21 01:28:18 2026 GMT
  host: buildots.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Buildots
provider_slug: buildots
slug: buildots-domain-security
source_filename: buildots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:28:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: buildots.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildots/refs/heads/main/security/buildots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction Tech
- ConTech
- Computer Vision
- AI
- Machine Learning
- Construction Progress
- 360 Camera
- BIM
- Project Management
- Schedule Tracking
- Risk Detection
- Deviation Detection
- Workforce Intelligence
- Capture Services
- Genda
- Tel Aviv
- Israel
---
