---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marinsoftware.com
  spf: true
hosts:
- cert_expires: Sep 10 03:10:25 2026 GMT
  host: www.marinsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marin Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marin Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marin Software
provider_slug: marin-software
slug: marin-software-domain-security
source_filename: marin-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marinsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:10:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marinsoftware.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marin-software/refs/heads/main/security/marin-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Advertising
- Marketing
- Performance Marketing
- Digital Advertising
- Paid Search
- Paid Social
- Retail Media
---
