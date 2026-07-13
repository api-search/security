---
api_specs:
- filename: medplum-openapi-original.yml
  format: yaml
  label: Medplum FHIR REST API
  slug: medplum-fhir-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/openapi/medplum-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medplum.com
  spf: true
hosts:
- cert_expires: Aug 22 08:42:13 2026 GMT
  host: www.medplum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.medplum.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medplum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medplum, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medplum
provider_slug: medplum
slug: medplum-domain-security
source_filename: medplum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.medplum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: medplum.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medplum/refs/heads/main/security/medplum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- Open Source
- Developer Platform
- HIPAA
- SMART on FHIR
- Clinical
- Interoperability
---
