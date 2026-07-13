---
api_specs:
- filename: client-api-external
  format: yaml
  label: AlayaCare Client API
  slug: alayacare-client-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/AlayaCare/client-api-external
- filename: alayacare-scheduler-openapi.yml
  format: yaml
  label: AlayaCare Scheduler API
  slug: alayacare-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-scheduler-openapi.yml
- filename: alayacare-forms-openapi.yml
  format: yaml
  label: AlayaCare Forms API
  slug: alayacare-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-forms-openapi.yml
- filename: alayacare-accounting-openapi.yml
  format: yaml
  label: AlayaCare Accounting API
  slug: alayacare-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/openapi/alayacare-accounting-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:team-badwolf@alayacare.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alayacare.com
  spf: true
hosts:
- cert_expires: Aug 18 11:43:59 2026 GMT
  host: alayacare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.prod.alayacare.com
  https: false
- cert_expires: Oct  3 21:27:20 2026 GMT
  host: acresi-api-docs.residential.alayacare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alayacare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlayaCare, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AlayaCare
provider_slug: api-evangelist-alayacare
slug: alayacare-domain-security
source_filename: alayacare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alayacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 11:43:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prod.alayacare.com\n  https: false\n- host: acresi-api-docs.residential.alayacare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:27:20 2026 GMT\n  hsts: false\ndomains:\n- domain: alayacare.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:team-badwolf@alayacare.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-alayacare/refs/heads/main/security/alayacare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Care
- Community Care
- Healthcare
- Scheduling
- Clinical
- Billing
- Client Management
- Care Management
- Aged Care
- Workforce Management
---
