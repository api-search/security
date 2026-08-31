---
api_specs:
- filename: asknicely-contacts-api-openapi.yml
  format: yaml
  label: AskNicely Contacts API
  slug: asknicely-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-contacts-api-openapi.yml
- filename: asknicely-in-app-surveys-api-openapi.yml
  format: yaml
  label: AskNicely In-App Surveys API
  slug: asknicely-in-app-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-in-app-surveys-api-openapi.yml
- filename: asknicely-responses-api-openapi.yml
  format: yaml
  label: AskNicely Responses API
  slug: asknicely-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-responses-api-openapi.yml
- filename: asknicely-statistics-api-openapi.yml
  format: yaml
  label: AskNicely Statistics API
  slug: asknicely-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-statistics-api-openapi.yml
- filename: asknicely-surveys-api-openapi.yml
  format: yaml
  label: AskNicely Surveys API
  slug: asknicely-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-surveys-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asknicely.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asknice.ly
  spf: true
hosts:
- cert_expires: Oct 22 08:56:37 2026 GMT
  host: www.asknicely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: demo.asknice.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 10:54:17 2026 GMT
  host: asknicely.zendesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asknicely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AskNicely, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AskNicely
provider_slug: asknicely
slug: asknicely-domain-security
source_filename: asknicely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asknicely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 08:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.asknice.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: asknicely.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 10:54:17 2026 GMT\n  hsts: null\ndomains:\n- domain: asknicely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: asknice.ly\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/security/asknicely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Experience
- Net Promoter Score
- Surveys
- Feedback
- Reputation Management
- Software-as-a-Service
- Customer Success
- Reviews
- SMS
---
