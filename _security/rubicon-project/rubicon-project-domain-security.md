---
api_specs:
- filename: rubicon-project-springserve-v1-openapi.yml
  format: yaml
  label: SpringServe UI API (v1)
  slug: rubicon-project-springserve-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v1-openapi.yml
- filename: rubicon-project-springserve-v0-openapi.yml
  format: yaml
  label: SpringServe UI API (v0)
  slug: rubicon-project-springserve-v0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v0-openapi.yml
- filename: rubicon-project-springserve-v1-openapi.yml
  format: yaml
  label: ClearLine API
  slug: rubicon-project-clearline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/openapi/rubicon-project-springserve-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magnite.com
  spf: true
- caa:
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Sep  4 17:48:00 2026 GMT
  host: www.magnite.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: springserve.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: console.springserve.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rubicon Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rubicon Project, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rubicon Project
provider_slug: rubicon-project
slug: rubicon-project-domain-security
source_filename: rubicon-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magnite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: springserve.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.springserve.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magnite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue\
  \ \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/security/rubicon-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Programmatic Advertising
- Sell-Side Platform
- SSP
- Real-Time Bidding
- Connected TV
- Ad Serving
- Media
- OpenRTB
- Reporting
---
