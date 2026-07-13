---
api_specs:
- filename: core.json
  format: json
  label: Stedi Core API
  slug: stedi-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/core.json
- filename: healthcare.json
  format: json
  label: Stedi Healthcare Eligibility API
  slug: stedi-healthcare-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/healthcare.json
- filename: claims.json
  format: json
  label: Stedi Claims API
  slug: stedi-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/claims.json
- filename: payers.json
  format: json
  label: Stedi Payers API
  slug: stedi-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/payers.json
- filename: enrollment.json
  format: json
  label: Stedi Enrollment API
  slug: stedi-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/enrollment.json
- filename: event-destinations.json
  format: json
  label: Stedi Event Destinations API
  slug: stedi-event-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Stedi/openApi/main/event-destinations.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stedi.com
  spf: true
hosts:
- cert_expires: Sep 23 03:39:35 2026 GMT
  host: www.stedi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: core.us.stedi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: healthcare.us.stedi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stedi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stedi
provider_slug: stedi
slug: stedi-domain-security
source_filename: stedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:39:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core.us.stedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: healthcare.us.stedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stedi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stedi/refs/heads/main/security/stedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EDI
- Electronic Data Interchange
- Healthcare
- Clearinghouse
- X12
- Claims
- Eligibility
- HIPAA
- Revenue Cycle Management
- B2B Integration
---
