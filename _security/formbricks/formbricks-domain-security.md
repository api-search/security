---
api_specs:
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Surveys API
  slug: surveys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Responses API
  slug: responses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Contacts and Attributes API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
- filename: formbricks-openapi.yml
  format: yaml
  label: Formbricks Management API
  slug: management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/openapi/formbricks-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: formbricks.com
  spf: true
hosts:
- cert_expires: Oct  1 14:53:06 2026 GMT
  host: www.formbricks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:53:06 2026 GMT
  host: formbricks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:53:06 2026 GMT
  host: app.formbricks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formbricks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formbricks, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Formbricks
provider_slug: formbricks
slug: formbricks-domain-security
source_filename: formbricks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.formbricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:53:06 2026 GMT\n  hsts: null\n- host: formbricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:53:06 2026 GMT\n  hsts: false\n- host: app.formbricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:53:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: formbricks.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formbricks/refs/heads/main/security/formbricks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Surveys
- Experience Management
- Feedback
- Forms
- Open Source
---
