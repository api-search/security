---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flosports.tv
  spf: true
hosts:
- cert_expires: Sep 25 15:16:48 2026 GMT
  host: www.flosports.tv
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flosports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FloSports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FloSports
provider_slug: flosports
slug: flosports-domain-security
source_filename: flosports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flosports.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:16:48 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: flosports.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flosports/refs/heads/main/security/flosports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Media
- Streaming
- Sports
- Video
- Entertainment
- Subscription
---
