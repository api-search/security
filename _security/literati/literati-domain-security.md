---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: literati.com
  spf: true
hosts:
- cert_expires: Aug 20 17:16:47 2026 GMT
  host: literati.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Literati Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Literati, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Literati
provider_slug: literati
slug: literati-domain-security
source_filename: literati-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: literati.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 17:16:47 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: literati.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/literati/refs/heads/main/security/literati-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Books
- Publishing
- Education
- Children
- Subscription Commerce
- Ecommerce
- Fundraising
- Schools
- Reading
---
