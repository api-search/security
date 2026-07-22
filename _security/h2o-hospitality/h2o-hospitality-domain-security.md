---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: h2ohospitality.io
  spf: true
hosts:
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: h2ohospitality.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: H2O Hospitality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H2O Hospitality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: H2O Hospitality
provider_slug: h2o-hospitality
slug: h2o-hospitality-domain-security
source_filename: h2o-hospitality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: h2ohospitality.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: h2ohospitality.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h2o-hospitality/refs/heads/main/security/h2o-hospitality-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Hospitality
- Hotels
- Property Management
- Travel
- Revenue Management
- Digital Transformation
- South Korea
---
