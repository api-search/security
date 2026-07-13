---
api_specs:
- filename: tenet-healthcare-fhir-openapi.yml
  format: yaml
  label: Tenet Health Patient Portal API
  slug: tenet-health-patient-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/openapi/tenet-healthcare-fhir-openapi.yml
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
