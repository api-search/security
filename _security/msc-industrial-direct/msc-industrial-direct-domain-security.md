---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mscdirect.com
  spf: true
hosts:
- cert_expires: Oct  8 12:54:36 2026 GMT
  host: www.mscdirect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Msc Industrial Direct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MSC Industrial Direct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MSC Industrial Direct
provider_slug: msc-industrial-direct
slug: msc-industrial-direct-domain-security
source_filename: msc-industrial-direct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mscdirect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:54:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mscdirect.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/msc-industrial-direct/refs/heads/main/security/msc-industrial-direct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distribution
- Industrial
- Maintenance
- Manufacturing
- Metalworking
- MRO
- Procurement
- Fortune 1000
---
