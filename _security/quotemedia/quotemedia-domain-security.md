---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: quotemedia.com
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: quotemedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:28:11 2026 GMT
  host: www.quotemedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: app.quotemedia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quotemedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuoteMedia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: QuoteMedia
provider_slug: quotemedia
slug: quotemedia-domain-security
source_filename: quotemedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quotemedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: www.quotemedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:28:11 2026 GMT\n  hsts: false\n- host: app.quotemedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quotemedia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quotemedia/refs/heads/main/security/quotemedia-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Stocks
- Options
- Real-Time
- Streaming
- News
- Fundamentals
- Reference Data
---
