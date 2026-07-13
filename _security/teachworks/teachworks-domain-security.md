---
api_specs:
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Customers API
  slug: teachworks-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Students API
  slug: teachworks-students-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Employees API
  slug: teachworks-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Lessons API
  slug: teachworks-lessons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Events and Availability API
  slug: teachworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Services and Subjects API
  slug: teachworks-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Invoices API
  slug: teachworks-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Payments API
  slug: teachworks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Wages API
  slug: teachworks-wages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
- filename: teachworks-openapi.yml
  format: yaml
  label: Teachworks Results and Repertoires API
  slug: teachworks-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/openapi/teachworks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teachworks.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Oct  1 23:48:20 2026 GMT
  host: teachworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:45:20 2026 GMT
  host: api.teachworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teachworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teachworks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teachworks
provider_slug: teachworks
slug: teachworks-domain-security
source_filename: teachworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teachworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.teachworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:45:20 2026 GMT\n  hsts: null\ndomains:\n- domain: teachworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/security/teachworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Tutoring
- EdTech
- Scheduling
- Business Management
- CRM
- Billing
---
