---
api_specs:
- filename: cloudrf-openapi.yml
  format: yaml
  label: CloudRF API
  slug: cloudrf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/openapi/cloudrf-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudrf.com
  spf: true
hosts:
- cert_expires: Aug 15 00:38:08 2026 GMT
  host: cloudrf.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:07:12 2026 GMT
  host: api.cloudrf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: dev.cloudrf.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cloudrf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudRF, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CloudRF
provider_slug: cloudrf
slug: cloudrf-domain-security
source_filename: cloudrf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudrf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 00:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.cloudrf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:07:12 2026 GMT\n  hsts: false\n- host: dev.cloudrf.com\n  https: false\ndomains:\n- domain: cloudrf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudrf/refs/heads/main/security/cloudrf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coverage Modeling
- HF Propagation
- Mesh Network
- Radio Frequency
- RF
- Satellite
- Signal Analysis
- Telecommunications
- Wireless Planning
---
