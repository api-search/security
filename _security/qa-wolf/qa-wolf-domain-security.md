---
api_specs:
- filename: qa-wolf-rest-openapi.yml
  format: yaml
  label: QA Wolf REST API
  slug: qa-wolf-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qa-wolf/refs/heads/main/openapi/qa-wolf-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qawolf.com
  spf: true
hosts:
- cert_expires: Sep 11 14:42:25 2026 GMT
  host: www.qawolf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qa Wolf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QA Wolf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QA Wolf
provider_slug: qa-wolf
slug: qa-wolf-domain-security
source_filename: qa-wolf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qawolf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:42:25 2026 GMT\n  hsts: false\ndomains:\n- domain: qawolf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qa-wolf/refs/heads/main/security/qa-wolf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Devtools
- Testing
- Test Automation
- QA
- CI/CD
- Playwright
- Developer Tools
---
