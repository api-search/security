---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bookkeepingexpress.com
  spf: true
hosts:
- cert_expires: Dec  3 14:08:38 2026 GMT
  host: bookkeepingexpress.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bookkeeping Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BookKeeping Express, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BookKeeping Express
provider_slug: bookkeeping-express
slug: bookkeeping-express-domain-security
source_filename: bookkeeping-express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bookkeepingexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 14:08:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: bookkeepingexpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bookkeeping-express/refs/heads/main/security/bookkeeping-express-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Bookkeeping
- Financial Coaching
- Small Business
- Software-as-a-Service
---
