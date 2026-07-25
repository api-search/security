---
api_specs:
- filename: overview
  format: yaml
  label: Moody's RMS Platform APIs
  slug: platform-apis
  spec_type: Postman
  url: https://www.postman.com/rms-developers/rms-developers/overview
- filename: moodys-rms-risk-modeler-openapi.yml
  format: yaml
  label: Moody's RMS Risk Modeler API
  slug: risk-modeler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-risk-modeler-openapi.yml
- filename: moodys-rms-data-bridge-openapi.json
  format: json
  label: Moody's RMS Data Bridge API
  slug: data-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-data-bridge-openapi.json
- filename: moodys-rms-location-intelligence-openapi.yaml
  format: yaml
  label: Moody's RMS Location Intelligence API
  slug: location-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/openapi/moodys-rms-location-intelligence-openapi.yaml
- filename: 21620294-578a748b-78a6-4a3a-b4b3-5c5380b7848e
  format: yaml
  label: Moody's RMS Climate On Demand API
  slug: climate-on-demand-api
  spec_type: Postman
  url: https://www.postman.com/rms-developers/workspace/cod/collection/21620294-578a748b-78a6-4a3a-b4b3-5c5380b7848e
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moodys.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rms.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.moodys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:57:38 2026 GMT
  host: developer.rms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 12:54:58 2026 GMT
  host: api-use1.rms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moodys Rms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moody''s RMS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moody's RMS
provider_slug: moodys-rms
slug: moodys-rms-domain-security
source_filename: moodys-rms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moodys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.rms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:57:38 2026 GMT\n  hsts: null\n- host: api-use1.rms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:54:58 2026 GMT\n  hsts: null\ndomains:\n- domain: moodys.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rms.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys-rms/refs/heads/main/security/moodys-rms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United States
- Property and Casualty
- Reinsurance
- Risk Data
- Catastrophe Modeling
- Underwriting
- Climate Risk
- Geocoding
- Analytics
---
