---
api_specs:
- filename: greenspark-openapi.yml
  format: yaml
  label: Greenspark Climate API
  slug: greenspark-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/openapi/greenspark-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getgreenspark.com
  spf: true
hosts:
- cert_expires: Oct 15 23:54:23 2026 GMT
  host: api.getgreenspark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:42:57 2026 GMT
  host: sandbox.getgreenspark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 16:31:04 2026 GMT
  host: demo-api.getgreenspark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenspark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenspark, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Greenspark
provider_slug: greenspark
slug: greenspark-domain-security
source_filename: greenspark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.getgreenspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:54:23 2026 GMT\n  hsts: null\n- host: sandbox.getgreenspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:42:57 2026 GMT\n  hsts: null\n- host: demo-api.getgreenspark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:31:04 2026 GMT\n  hsts: null\ndomains:\n- domain: getgreenspark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenspark/refs/heads/main/security/greenspark-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sustainability
- Carbon Offset
- Climate
- Impact
- Carbon Estimation
- Reporting
- ESG
- Fintech
---
