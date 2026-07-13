---
api_specs:
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Clients API
  slug: provet-cloud-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Patients API
  slug: provet-cloud-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Appointments API
  slug: provet-cloud-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Consultations API
  slug: provet-cloud-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Billing & Invoicing API
  slug: provet-cloud-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Items & Reference Data API
  slug: provet-cloud-items-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
- filename: provet-cloud-openapi.yml
  format: yaml
  label: Provet Cloud Webhooks API
  slug: provet-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/openapi/provet-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: provet.cloud
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: provetcloud.com
  spf: true
hosts:
- cert_expires: Aug 13 19:19:34 2026 GMT
  host: www.provet.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: developers.provetcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provet Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provet Cloud, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Provet Cloud
provider_slug: provet-cloud
slug: provet-cloud-domain-security
source_filename: provet-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.provet.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.provetcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: provet.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: provetcloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provet-cloud/refs/heads/main/security/provet-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Veterinary
- Practice Management
- PIMS
- Healthcare
- Nordhealth
- Animal Health
- Appointments
- Billing
---
