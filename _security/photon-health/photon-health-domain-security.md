---
api_specs:
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Patients API
  slug: photon-health-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Prescriptions API
  slug: photon-health-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Orders API
  slug: photon-health-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Catalog & Medications API
  slug: photon-health-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Pharmacies API
  slug: photon-health-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
- filename: photon-health-openapi.yml
  format: yaml
  label: Photon Health Webhooks API
  slug: photon-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/openapi/photon-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: photon.health
  spf: true
hosts:
- cert_expires: Oct  3 20:37:37 2026 GMT
  host: www.photon.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 04:40:29 2026 GMT
  host: docs.photon.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.photon.health
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photon Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Photon Health
provider_slug: photon-health
slug: photon-health-domain-security
source_filename: photon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.photon.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:37:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.photon.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 04:40:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.photon.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: photon.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon-health/refs/heads/main/security/photon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- e-Prescribing
- eRx
- Prescriptions
- Pharmacy
- GraphQL
---
