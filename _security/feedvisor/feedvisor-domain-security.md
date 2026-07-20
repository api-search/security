---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feedvisor.com
  spf: true
hosts:
- cert_expires: Aug 19 07:58:34 2026 GMT
  host: feedvisor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.feedvisor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feedvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feedvisor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Feedvisor
provider_slug: feedvisor
slug: feedvisor-domain-security
source_filename: feedvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feedvisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:58:34 2026 GMT\n  hsts: false\n- host: api.feedvisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: feedvisor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feedvisor/refs/heads/main/security/feedvisor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Amazon
- E-Commerce
- Retail
- Advertising
- Pricing
- Repricing
- Marketplace
- Machine Learning
- Optimization
---
