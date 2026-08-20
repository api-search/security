---
api_specs:
- filename: sun-life-dentaquest-fhir-patient-access-openapi.json
  format: json
  label: DentaQuest FHIR Patient Access API
  slug: sun-life-dentaquest-fhir-patient-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-patient-access-openapi.json
- filename: sun-life-dentaquest-fhir-provider-directory-openapi.json
  format: json
  label: DentaQuest FHIR Provider Directory API
  slug: sun-life-dentaquest-fhir-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-provider-directory-openapi.json
- filename: sun-life-dentaquest-fhir-metadata-openapi.json
  format: json
  label: DentaQuest FHIR Metadata API
  slug: sun-life-dentaquest-fhir-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/openapi/sun-life-dentaquest-fhir-metadata-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sunlife.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dentaquest.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: www.sunlife.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.dentaquest.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.deltadentalma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sun Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sun Life, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sun Life
provider_slug: sun-life
slug: sun-life-domain-security
source_filename: sun-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dentaquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: api.deltadentalma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sunlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dentaquest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sun-life/refs/heads/main/security/sun-life-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Life Insurance
- Health Insurance
- Employee Benefits
- Group Benefits
- Dental Insurance
- Disability
- Wealth Management
- Financial-Services
- Carrier
- FHIR
- Patient Access
- Provider Directory
- Healthcare Interoperability
- CMS-9115-F
- DentaQuest
- SMART on FHIR
- Dental Benefits
---
