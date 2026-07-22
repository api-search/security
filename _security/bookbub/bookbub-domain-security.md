---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bookbub.com
  spf: true
hosts:
- cert_expires: Sep 13 10:50:41 2026 GMT
  host: www.bookbub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bookbub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bookbub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bookbub
provider_slug: bookbub
slug: bookbub-domain-security
source_filename: bookbub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bookbub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:50:41 2026 GMT\n  hsts: null\ndomains:\n- domain: bookbub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookbub/refs/heads/main/security/bookbub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Books
- Publishing
- Ebooks
- Reading
- Book Discovery
- Author Marketing
- Advertising
- Media
- Consumer
---
