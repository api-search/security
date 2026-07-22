---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mybirdbuddy.com
  spf: true
hosts:
- cert_expires: Sep  2 02:20:45 2026 GMT
  host: mybirdbuddy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Birdbuddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BirdBuddy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BirdBuddy
provider_slug: birdbuddy
slug: birdbuddy-domain-security
source_filename: birdbuddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybirdbuddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:20:45 2026 GMT\n  hsts: false\ndomains:\n- domain: mybirdbuddy.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/birdbuddy/refs/heads/main/security/birdbuddy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Consumer Hardware
- Smart Home
- IoT
- Birding
- Computer Vision
- Mobile App
- GraphQL
---
