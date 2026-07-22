---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:tech@clubzero.co"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clubzero.co
  spf: true
hosts:
- cert_expires: Oct  4 14:00:36 2026 GMT
  host: clubzero.co
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clubzero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CLUBZERO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CLUBZERO
provider_slug: clubzero
slug: clubzero-domain-security
source_filename: clubzero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clubzero.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:00:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: clubzero.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:tech@clubzero.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clubzero/refs/heads/main/security/clubzero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reuse System
- Reusable Packaging
- Returnable Packaging
- Circular Economy
- Sustainability
- Food and Beverage
- Packaging
- Serialization
- Logistics
---
