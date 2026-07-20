---
api_specs:
- filename: catchpoint-systems-rest-api-v2-openapi.json
  format: json
  label: Catchpoint REST API v2
  slug: catchpoint-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/catchpoint-systems/refs/heads/main/openapi/catchpoint-systems-rest-api-v2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: catchpoint.com
  spf: true
hosts:
- cert_expires: Sep 25 17:36:35 2026 GMT
  host: docs.catchpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:49:01 2026 GMT
  host: io.catchpoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catchpoint Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catchpoint Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Catchpoint Systems
provider_slug: catchpoint-systems
slug: catchpoint-systems-domain-security
source_filename: catchpoint-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.catchpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:36:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: io.catchpoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:49:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: catchpoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catchpoint-systems/refs/heads/main/security/catchpoint-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Monitoring
- Observability
- Internet Performance Monitoring
- Synthetic Monitoring
- Real User Monitoring
- Network Monitoring
- Digital Experience Monitoring
- APIs
---
