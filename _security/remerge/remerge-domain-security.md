---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: remerge.io
  spf: true
hosts:
- cert_expires: Oct  5 12:17:47 2026 GMT
  host: www.remerge.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remerge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remerge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Remerge
provider_slug: remerge
slug: remerge-domain-security
source_filename: remerge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remerge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:17:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: remerge.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remerge/refs/heads/main/security/remerge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advertising
- AdTech
- Mobile
- Retargeting
- Demand-Side Platform
- User Acquisition
- Marketing
---
