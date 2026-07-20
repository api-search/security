---
api_specs:
- filename: leankit-agileplace-api-openapi.yml
  format: yaml
  label: Planview AgilePlace API (LeanKit) v2
  slug: agileplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/openapi/leankit-agileplace-api-openapi.yml
- filename: leankit-user-provisioning-api-openapi.yml
  format: yaml
  label: Planview AgilePlace User Provisioning API (SCIM 1.1)
  slug: user-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/openapi/leankit-user-provisioning-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: planview.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: leankit.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.planview.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: success.planview.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: myaccount.leankit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leankit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanKit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LeanKit
provider_slug: leankit
slug: leankit-domain-security
source_filename: leankit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: success.planview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: myaccount.leankit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: planview.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: leankit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/security/leankit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Kanban
- Project Management
- Agile
- Work Management
- Collaboration
- Enterprise Software
- Portfolio Management
- Workflow Automation
- SaaS
---
