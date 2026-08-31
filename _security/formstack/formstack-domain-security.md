---
api_specs:
- filename: formstack-asyncapi.yml
  format: yaml
  label: Formstack Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-asyncapi.yml
- filename: formstack-confirmations-api-openapi.yml
  format: yaml
  label: Formstack Confirmations API
  slug: formstack-confirmations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-confirmations-api-openapi.yml
- filename: formstack-fields-api-openapi.yml
  format: yaml
  label: Formstack Fields API
  slug: formstack-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-fields-api-openapi.yml
- filename: formstack-folders-api-openapi.yml
  format: yaml
  label: Formstack Folders API
  slug: formstack-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-folders-api-openapi.yml
- filename: formstack-forms-api-openapi.yml
  format: yaml
  label: Formstack Forms API
  slug: formstack-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-forms-api-openapi.yml
- filename: formstack-notifications-api-openapi.yml
  format: yaml
  label: Formstack Notifications API
  slug: formstack-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-notifications-api-openapi.yml
- filename: formstack-subaccounts-api-openapi.yml
  format: yaml
  label: Formstack Subaccounts API
  slug: formstack-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-subaccounts-api-openapi.yml
- filename: formstack-submissions-api-openapi.yml
  format: yaml
  label: Formstack Submissions API
  slug: formstack-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-submissions-api-openapi.yml
- filename: formstack-webhooks-api-openapi.yml
  format: yaml
  label: Formstack Webhooks API
  slug: formstack-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formstack.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webmerge.me
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.formstack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 22:13:28 2026 GMT
  host: developers.formstack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.webmerge.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Formstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formstack, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Formstack
provider_slug: formstack
slug: formstack-domain-security
source_filename: formstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.formstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.formstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 22:13:28 2026 GMT\n  hsts: null\n- host: www.webmerge.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: formstack.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: webmerge.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/security/formstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Documents
- eSignature
- Workflow-Automation
- No-Code
- Authentication
---
