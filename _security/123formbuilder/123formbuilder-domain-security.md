---
api_specs:
- filename: 123formbuilder-rest-api-v2-openapi.yml
  format: yaml
  label: 123FormBuilder REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/123formbuilder/refs/heads/main/openapi/123formbuilder-rest-api-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:devteam@123contactform.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 123formbuilder.com
  spf: true
hosts:
- cert_expires: Sep  5 09:09:14 2026 GMT
  host: www.123formbuilder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.123formbuilder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: eu-api.123formbuilder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 123Formbuilder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 123FormBuilder, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 123FormBuilder
provider_slug: 123formbuilder
slug: 123formbuilder-domain-security
source_filename: 123formbuilder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.123formbuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 09:09:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.123formbuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\n- host: eu-api.123formbuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: 123formbuilder.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:devteam@123contactform.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/123formbuilder/refs/heads/main/security/123formbuilder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Online Forms
- Form Builder
- Surveys
- Workflow
- Data Collection
- Submissions
- Webhooks
- HIPAA
- GDPR
- Payments
---
