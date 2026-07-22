---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ke.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: ke.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Beike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beike, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beike
provider_slug: beike
slug: beike-domain-security
source_filename: beike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ke.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beike/refs/heads/main/security/beike-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Technology
- Real Estate
- Housing
- Property
- Marketplace
- Consumer
- China
---
