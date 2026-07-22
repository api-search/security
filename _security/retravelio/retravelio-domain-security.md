---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: retravel.io
  spf: true
hosts:
- cert_expires: Sep 25 06:01:46 2026 GMT
  host: retravel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retravelio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for reTravel.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: reTravel.io
provider_slug: retravelio
slug: retravelio-domain-security
source_filename: retravelio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retravel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:01:46 2026 GMT\n  hsts: false\ndomains:\n- domain: retravel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retravelio/refs/heads/main/security/retravelio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Travel Technology
- Marketing
- Customer Retention
- Machine Learning
- Personalization
---
