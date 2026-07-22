---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kabam.com
  spf: true
hosts:
- cert_expires: Oct 12 20:30:52 2026 GMT
  host: kabam.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kabam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kabam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kabam
provider_slug: kabam
slug: kabam-domain-security
source_filename: kabam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kabam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 20:30:52 2026 GMT\n  hsts: null\ndomains:\n- domain: kabam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kabam/refs/heads/main/security/kabam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Mobile Games
- Video Games
- Entertainment
- Mobile
---
