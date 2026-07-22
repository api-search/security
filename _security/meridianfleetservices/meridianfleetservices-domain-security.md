---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meridianfleetservices.com
  spf: true
hosts:
- cert_expires: Aug 21 01:55:59 2026 GMT
  host: meridianfleetservices.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meridianfleetservices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meridianfleetservices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meridianfleetservices
provider_slug: meridianfleetservices
slug: meridianfleetservices-domain-security
source_filename: meridianfleetservices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meridianfleetservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meridianfleetservices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meridianfleetservices/refs/heads/main/security/meridianfleetservices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fleet Services
- Fleet Management
- Transportation
- Holding Company
- Acquisitions
---
