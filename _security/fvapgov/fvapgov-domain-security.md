---
api_specs:
- filename: fvapgov-xml-api-openapi.yml
  format: yaml
  label: FVAP.gov XML API
  slug: fvapgov-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fvapgov/refs/heads/main/openapi/fvapgov-xml-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fvap.gov
  spf: true
hosts:
- cert_expires: Sep 23 17:36:54 2026 GMT
  host: www.fvap.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fvapgov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FVAP.gov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FVAP.gov
provider_slug: fvapgov
slug: fvapgov-domain-security
source_filename: fvapgov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fvap.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 17:36:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fvap.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fvapgov/refs/heads/main/security/fvapgov-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Government
- Voting
---
