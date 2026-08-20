---
api_specs:
- filename: santeacademie-frontstage-openapi.json
  format: json
  label: Santé Académie Frontstage API
  slug: santé-académie-frontstage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-frontstage-openapi.json
- filename: santeacademie-connector-openapi.json
  format: json
  label: Santé Académie Connector API
  slug: santé-académie-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-connector-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: santeacademie.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.santeacademie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 04:26:04 2026 GMT
  host: frontstage.santeacademie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santeacademie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santé Académie, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Santé Académie
provider_slug: santeacademie
slug: santeacademie-domain-security
source_filename: santeacademie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.santeacademie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: frontstage.santeacademie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 04:26:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: santeacademie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/security/santeacademie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EdTech
- Healthcare Training
- Continuing Education
- DPC
- E-Learning
- France
- Healthcare Professionals
- Course Catalog
- LMS
---
