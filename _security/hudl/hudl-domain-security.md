---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:infrastructure@hudl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hudl.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.hudl.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hudl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hudl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hudl
provider_slug: hudl
slug: hudl-domain-security
source_filename: hudl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hudl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: hudl.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:infrastructure@hudl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hudl/refs/heads/main/security/hudl-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Sports
- Sports Technology
- Sports Performance
- Sports Analytics
- Video Analysis
- Performance Analysis
- Video Capture
- AI Cameras
- Coaching
- Team Management
- Football Analytics
- Soccer Analytics
- Basketball
- Volleyball
- American Football
- Wyscout
- Statsbomb
- Sportscode
- Athlete Tracking
- Livestreaming
- Ticketing
- Sports Data
---
