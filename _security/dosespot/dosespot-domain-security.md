---
api_specs:
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Patients API
  slug: dosespot-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescriptions API
  slug: dosespot-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Medications API
  slug: dosespot-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Pharmacies API
  slug: dosespot-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Prescribers API
  slug: dosespot-prescribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
- filename: dosespot-openapi.yml
  format: yaml
  label: DoseSpot Notifications API
  slug: dosespot-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dosespot.com
  spf: true
hosts:
- cert_expires: Oct  9 07:18:35 2026 GMT
  host: www.dosespot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:02:47 2026 GMT
  host: dosespot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: my.dosespot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dosespot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoseSpot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DoseSpot
provider_slug: dosespot
slug: dosespot-domain-security
source_filename: dosespot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dosespot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:18:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dosespot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.dosespot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dosespot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/security/dosespot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- e-Prescribing
- eRx
- Healthcare
- EHR
- Pharmacy
- EPCS
---
