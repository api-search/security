---
api_specs:
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Sandbox FHIR R4 API
  slug: smarthealthit-sandbox-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART App Launch Authorization API
  slug: smarthealthit-smart-app-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
- filename: smarthealthit-openapi.yml
  format: yaml
  label: SMART Bulk Data Export API
  slug: smarthealthit-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/openapi/smarthealthit-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smarthealthit.org
  spf: true
hosts:
- cert_expires: Aug 18 08:44:01 2026 GMT
  host: smarthealthit.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 16:23:57 2026 GMT
  host: r4.smarthealthit.org
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 17 23:24:48 2026 GMT
  host: launch.smarthealthit.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smarthealthit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMART Health IT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMART Health IT
provider_slug: smarthealthit
slug: smarthealthit-domain-security
source_filename: smarthealthit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smarthealthit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:44:01 2026 GMT\n  hsts: false\n- host: r4.smarthealthit.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 16:23:57 2026 GMT\n  hsts: null\n- host: launch.smarthealthit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:24:48 2026 GMT\n  hsts: false\ndomains:\n- domain: smarthealthit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthealthit/refs/heads/main/security/smarthealthit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMART on FHIR
- FHIR
- Health IT
- EHR Integration
- Clinical Data
- Clinical Records
- Patient Facing
- Open Standards
- Interoperability
---
