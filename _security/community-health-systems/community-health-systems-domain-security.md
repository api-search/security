---
api_specs:
- filename: chs-patient-access-api-openapi.yml
  format: yaml
  label: Community Health Systems Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/openapi/chs-patient-access-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chs.net
  spf: true
hosts:
- cert_expires: Jan 24 18:46:33 2027 GMT
  host: www.chs.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.chs.net
  https: false
kind: domain-security
layout: security
method: probed
name: Community Health Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Community Health Systems, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Community Health Systems
provider_slug: community-health-systems
slug: community-health-systems-domain-security
source_filename: community-health-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chs.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 18:46:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chs.net\n  https: false\ndomains:\n- domain: chs.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/security/community-health-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS-9115-F
- FHIR
- Healthcare
- Hospitals
- Interoperability
- Patient Access
- Provider Directory
- SMART-on-FHIR
- Fortune 500
---
