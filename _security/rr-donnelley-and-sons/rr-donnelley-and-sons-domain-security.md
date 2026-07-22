---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rrd.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.rrd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rr Donnelley And Sons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RR Donnelley And Sons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RR Donnelley And Sons
provider_slug: rr-donnelley-and-sons
slug: rr-donnelley-and-sons-domain-security
source_filename: rr-donnelley-and-sons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rrd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rrd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rr-donnelley-and-sons/refs/heads/main/security/rr-donnelley-and-sons-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Communications
- Marketing
- Print Services
- Direct Mail
- Logistics
- Fortune 1000
---
