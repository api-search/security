---
api_specs:
- filename: mine-openapi-original.json
  format: json
  label: MineOS API
  slug: mineos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-openapi-original.json
- filename: mine-partners-openapi-original.json
  format: json
  label: MineOS Partners API
  slug: mineos-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/openapi/mine-partners-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mineos.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: saymine.com
  spf: true
hosts:
- cert_expires: Aug 31 07:29:38 2026 GMT
  host: www.mineos.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 00:42:41 2026 GMT
  host: developers.mineos.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 18:17:53 2026 GMT
  host: api.portal.saymine.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MINE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MINE
provider_slug: mine
slug: mine-domain-security
source_filename: mine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mineos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:29:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.mineos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.portal.saymine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 18:17:53 2026 GMT\n  hsts: null\ndomains:\n- domain: mineos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: saymine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mine/refs/heads/main/security/mine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Privacy
- Data Governance
- Privacy Operations
- Consent Management
- AI Governance
- Third-Party Risk
- Compliance
- Security
---
