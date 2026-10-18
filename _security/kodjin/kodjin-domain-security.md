---
api_specs:
- filename: kodjin-auth-api-openapi.yml
  format: yaml
  label: Kodjin Auth API
  slug: kodjin-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kodjin/refs/heads/main/openapi/kodjin-auth-api-openapi.yml
- filename: kodjin-fhir-api-openapi.yml
  format: yaml
  label: Kodjin Fhir API
  slug: kodjin-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kodjin/refs/heads/main/openapi/kodjin-fhir-api-openapi.yml
- filename: kodjin-patient-api-openapi.yml
  format: yaml
  label: Kodjin Patient API
  slug: kodjin-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kodjin/refs/heads/main/openapi/kodjin-patient-api-openapi.yml
- filename: kodjin-terminology-api-openapi.yml
  format: yaml
  label: Kodjin Terminology API
  slug: kodjin-terminology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kodjin/refs/heads/main/openapi/kodjin-terminology-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kodjin.com
  spf: true
hosts:
- cert_expires: Jan  2 12:30:57 2027 GMT
  host: kodjin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kodjin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kodjin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kodjin
provider_slug: kodjin
slug: kodjin-domain-security
source_filename: kodjin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kodjin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 12:30:57 2027 GMT\n  hsts: false\ndomains:\n- domain: kodjin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodjin/refs/heads/main/security/kodjin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Low-code
- Platform
- Automation
- Integration
---
