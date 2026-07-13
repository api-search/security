---
api_specs:
- filename: freshbooks-openapi.yml
  format: yaml
  label: FreshBooks REST API
  slug: freshbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/openapi/freshbooks-openapi.yml
- filename: freshbooks-webhooks-asyncapi.yml
  format: yaml
  label: FreshBooks Webhooks (Callbacks API)
  slug: freshbooks-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/asyncapi/freshbooks-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: freshbooks.com
  spf: true
hosts:
- cert_expires: Oct  1 02:55:52 2026 GMT
  host: www.freshbooks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 01:44:32 2026 GMT
  host: api.freshbooks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshbooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreshBooks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FreshBooks
provider_slug: freshbooks
slug: freshbooks-domain-security
source_filename: freshbooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshbooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:55:52 2026 GMT\n  hsts: false\n- host: api.freshbooks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:44:32 2026 GMT\n  hsts: null\ndomains:\n- domain: freshbooks.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshbooks/refs/heads/main/security/freshbooks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Accounting
- Invoicing
- Expense Tracking
- Time Tracking
- Small Business
- Bookkeeping
---
