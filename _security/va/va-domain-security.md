---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/department-of-veterans-affairs/vets-api-clients/master/services/benefits-intake/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: va.gov
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developer.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.va.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Va Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veterans Affairs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Veterans Affairs
provider_slug: va
slug: va-domain-security
source_filename: va-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.va.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: va.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/security/va-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Veterans
- Government
- Health
- Benefits
- FHIR
- Appeals
- Federal
---
