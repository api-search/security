---
api_specs:
- filename: shyft-customer-openapi-original.json
  format: json
  label: Shyft Customer API
  slug: shyft-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shyft/refs/heads/main/openapi/shyft-customer-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myshyft.com
  spf: true
hosts:
- cert_expires: Oct  6 14:14:14 2026 GMT
  host: myshyft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:37:07 2026 GMT
  host: customer-api-doc.myshyft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:37:07 2026 GMT
  host: app.myshyft.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Shyft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shyft, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shyft
provider_slug: shyft
slug: shyft-domain-security
source_filename: shyft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myshyft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:14:14 2026 GMT\n  hsts: null\n- host: customer-api-doc.myshyft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:37:07 2026 GMT\n  hsts: false\n- host: app.myshyft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 18:37:07 2026 GMT\n  hsts: false\ndomains:\n- domain: myshyft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shyft/refs/heads/main/security/shyft-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Workforce Management
- Employee Scheduling
- Shift Swapping
- Team Communication
- Hourly Workers
- Earned Wage Access
- HR Tech
- REST API
---
