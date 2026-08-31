---
api_specs:
- filename: photon-agent-discovery-api-openapi.yml
  format: yaml
  label: Photon Agent discovery API
  slug: photon-agent-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-agent-discovery-api-openapi.yml
- filename: photon-newsletter-api-openapi.yml
  format: yaml
  label: Photon Newsletter API
  slug: photon-newsletter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-newsletter-api-openapi.yml
- filename: photon-onboarding-api-openapi.yml
  format: yaml
  label: Photon Onboarding API
  slug: photon-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-onboarding-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: photonhealth.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: photon.health
  spf: true
hosts:
- cert_expires: Oct 22 19:14:52 2026 GMT
  host: photonhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 05:50:35 2026 GMT
  host: docs.photon.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 19:35:47 2026 GMT
  host: clinical-api.photon.health
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Photon
provider_slug: photon
slug: photon-domain-security
source_filename: photon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: photonhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 19:14:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.photon.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:50:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: clinical-api.photon.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:35:47 2026 GMT\n  hsts: null\ndomains:\n- domain: photonhealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: photon.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/security/photon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- United States
- e-Prescribing
- Pharmacy
- Prescription Routing
- GraphQL
- Clinical API
- Digital Health
- Benefit Check
- Authentication
---
