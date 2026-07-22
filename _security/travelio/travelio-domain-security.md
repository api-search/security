---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: travelio.com
  spf: true
hosts:
- cert_expires: Aug 23 03:59:35 2026 GMT
  host: travelio.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travelio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Travelio
provider_slug: travelio
slug: travelio-domain-security
source_filename: travelio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: travelio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:59:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: travelio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelio/refs/heads/main/security/travelio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property Rental
- Real Estate
- Property Management
- Hospitality
- Travel
- Indonesia
- Apartments
---
