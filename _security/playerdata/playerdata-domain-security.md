---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: playerdata.co.uk
  spf: true
hosts:
- cert_expires: Oct 15 01:34:46 2026 GMT
  host: playerdata.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playerdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayerData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlayerData
provider_slug: playerdata
slug: playerdata-domain-security
source_filename: playerdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playerdata.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:34:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: playerdata.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playerdata/refs/heads/main/security/playerdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sports
- Sports Performance
- GPS Tracking
- Wearables
- Athlete Monitoring
- GraphQL
- Analytics
---
