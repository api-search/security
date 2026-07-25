---
api_specs:
- filename: openfda-animal-veterinary-api-openapi.yml
  format: yaml
  label: openFDA Animal & Veterinary API
  slug: openfda-animal-veterinary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-animal-veterinary-api-openapi.yml
- filename: openfda-device-api-openapi.yml
  format: yaml
  label: openFDA Device API
  slug: openfda-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-device-api-openapi.yml
- filename: openfda-drug-api-openapi.yml
  format: yaml
  label: openFDA Drug API
  slug: openfda-drug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-drug-api-openapi.yml
- filename: openfda-food-api-openapi.yml
  format: yaml
  label: openFDA Food API
  slug: openfda-food-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-food-api-openapi.yml
- filename: openfda-other-api-openapi.yml
  format: yaml
  label: openFDA Other API
  slug: openfda-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-other-api-openapi.yml
- filename: openfda-tobacco-api-openapi.yml
  format: yaml
  label: openFDA Tobacco API
  slug: openfda-tobacco-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/openapi/openfda-tobacco-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fda.gov
  spf: true
hosts:
- cert_expires: Oct  2 18:57:13 2026 GMT
  host: open.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:20:53 2026 GMT
  host: api.fda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openfda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openFDA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: openFDA
provider_slug: openfda
slug: openfda-domain-security
source_filename: openfda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:20:53 2026 GMT\n  hsts: null\ndomains:\n- domain: fda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfda/refs/heads/main/security/openfda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Healthcare
- Drug
- Device
- Food
- Animal & Veterinary
- Tobacco
- Public Data
- Open Data
- Adverse Events
- Recalls
- Regulatory
---
