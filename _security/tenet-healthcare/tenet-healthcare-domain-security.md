---
api_specs:
- filename: tenet-healthcare-appointments-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Appointments API
  slug: tenet-healthcare-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-appointments-api-openapi.yml
- filename: tenet-healthcare-conditions-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Conditions API
  slug: tenet-healthcare-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-conditions-api-openapi.yml
- filename: tenet-healthcare-documents-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Documents API
  slug: tenet-healthcare-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-documents-api-openapi.yml
- filename: tenet-healthcare-medications-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Medications API
  slug: tenet-healthcare-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-medications-api-openapi.yml
- filename: tenet-healthcare-observations-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Observations API
  slug: tenet-healthcare-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-observations-api-openapi.yml
- filename: tenet-healthcare-patients-api-openapi.yml
  format: yaml
  label: Tenet Healthcare Patients API
  slug: tenet-healthcare-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-patients-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tenethealth.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tenetcorporate.com
  spf: false
hosts:
- cert_expires: Oct  7 16:19:13 2026 GMT
  host: www.tenethealth.com
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
- host: www.tenetcorporate.com
  https: false
- cert_expires: Aug 12 12:44:18 2026 GMT
  host: www.coniferhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenet Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenet Healthcare, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tenet Healthcare
provider_slug: tenet-healthcare
slug: tenet-healthcare-domain-security
source_filename: tenet-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tenethealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\n- host: www.tenetcorporate.com\n  https: false\n- host: www.coniferhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:44:18 2026 GMT\n  hsts: null\ndomains:\n- domain: tenethealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tenetcorporate.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/security/tenet-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Hospitals
- Ambulatory Surgery Centers
- Revenue Cycle Management
- Fortune 500
---
