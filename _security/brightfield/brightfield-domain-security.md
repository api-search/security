---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brightfield.com
  spf: true
hosts:
- cert_expires: Sep 25 19:54:57 2026 GMT
  host: www.brightfield.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightfield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightfield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brightfield
provider_slug: brightfield
slug: brightfield-domain-security
source_filename: brightfield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightfield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:54:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brightfield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightfield/refs/heads/main/security/brightfield-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- Workforce Intelligence
- Contingent Workforce
- Procurement
- Analytics
- Statement of Work
---
