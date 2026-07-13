---
api_specs:
- filename: actionstep-actions-openapi.yml
  format: yaml
  label: Actionstep API
  slug: actionstep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actionstep/refs/heads/main/openapi/actionstep-actions-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 iodef "mailto:informationsecurity@actionstep.com"
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: actionstep.com
  spf: true
hosts:
- cert_expires: Aug 28 16:32:10 2026 GMT
  host: www.actionstep.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: docs.actionstep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.actionstep.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Actionstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actionstep, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Actionstep
provider_slug: actionstep
slug: actionstep-domain-security
source_filename: actionstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actionstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:32:10 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.actionstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.actionstep.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: actionstep.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 iodef \"mailto:informationsecurity@actionstep.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actionstep/refs/heads/main/security/actionstep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Practice Management
- Law Firm
- Matters
- Billing
- Documents
- Trust Accounting
- Contacts
- Workflow
---
