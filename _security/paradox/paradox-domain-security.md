---
api_specs:
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Conversational AI API
  slug: paradox-conversational-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Company API
  slug: paradox-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Candidates API
  slug: paradox-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Users API
  slug: paradox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Scheduling API
  slug: paradox-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Locations API
  slug: paradox-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Reporting API
  slug: paradox-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox Candidate Attributes API
  slug: paradox-candidate-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
- filename: paradox-api-openapi.yml
  format: yaml
  label: Paradox User Permissions API
  slug: paradox-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "www.digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:paradox-devops@workday.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paradox.ai
  spf: true
hosts:
- cert_expires: Aug 12 21:12:07 2026 GMT
  host: readme.paradox.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 14:56:36 2026 GMT
  host: www.paradox.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: api.paradox.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paradox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paradox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paradox
provider_slug: paradox
slug: paradox-domain-security
source_filename: paradox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readme.paradox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 21:12:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.paradox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:56:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paradox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paradox.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:paradox-devops@workday.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/security/paradox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Candidate Screening
- Chatbot
- Conversational AI
- Hiring Automation
- HR Technology
- Interview Scheduling
- Recruiting
- SMS
- Talent Acquisition
---
