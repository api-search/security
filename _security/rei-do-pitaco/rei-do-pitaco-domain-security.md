---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reidopitaco.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.reidopitaco.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rei Do Pitaco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rei do Pitaco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rei do Pitaco
provider_slug: rei-do-pitaco
slug: rei-do-pitaco-domain-security
source_filename: rei-do-pitaco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reidopitaco.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reidopitaco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rei-do-pitaco/refs/heads/main/security/rei-do-pitaco-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Sports Betting
- Fantasy Sports
- iGaming
- Casino
- Gambling
- Brazil
- Sports
---
