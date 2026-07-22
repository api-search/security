---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: percolata.com
  spf: true
hosts:
- cert_expires: Aug 24 17:10:01 2026 GMT
  host: percolata.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Percolata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Percolata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Percolata
provider_slug: percolata
slug: percolata-domain-security
source_filename: percolata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: percolata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:10:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: percolata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/percolata/refs/heads/main/security/percolata-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Retail
- Analytics
- Machine Learning
- Predictive Analytics
- Workforce Optimization
- Marketing Optimization
---
