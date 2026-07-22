---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rover.com
  spf: true
hosts:
- cert_expires: Aug 16 11:43:38 2026 GMT
  host: www.rover.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rover, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rover
provider_slug: rover
slug: rover-domain-security
source_filename: rover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:43:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: rover.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rover/refs/heads/main/security/rover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Care
- Dog Walking
- Pet Sitting
- Marketplace
- Consumer
- No Public API
- Stub
---
