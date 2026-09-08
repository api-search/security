---
api_specs:
- filename: asce-amplify-hazard-loads-openapi.yml
  format: yaml
  label: ASCE Hazard Tool API
  slug: hazard-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asce-amplify/refs/heads/main/openapi/asce-amplify-hazard-loads-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asce.org
  spf: true
hosts:
- cert_expires: Nov 24 02:35:49 2026 GMT
  host: www.asce.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 19:01:20 2026 GMT
  host: amplify.asce.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api-hazard.asce.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Asce Amplify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASCE Amplify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ASCE Amplify
provider_slug: asce-amplify
slug: asce-amplify-domain-security
source_filename: asce-amplify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 02:35:49 2026 GMT\n  hsts: false\n- host: amplify.asce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 19:01:20 2026 GMT\n  hsts: null\n- host: api-hazard.asce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: asce.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asce-amplify/refs/heads/main/security/asce-amplify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Civil Engineering
- Hazard Data
- Engineering Standards
- Infrastructure
- Structural Engineering
- Geospatial
- Seismic
- Building Codes
- Standards Body
---
