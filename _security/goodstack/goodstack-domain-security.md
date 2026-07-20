---
api_specs:
- filename: goodstack-openapi-original.json
  format: json
  label: Goodstack Services
  slug: goodstack-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodstack/refs/heads/main/openapi/goodstack-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: goodstack.io
  spf: true
hosts:
- cert_expires: Aug 19 20:03:00 2026 GMT
  host: docs.goodstack.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.goodstack.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: sandbox-api.goodstack.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodstack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Goodstack
provider_slug: goodstack
slug: goodstack-domain-security
source_filename: goodstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.goodstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:03:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goodstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\n- host: sandbox-api.goodstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goodstack.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodstack/refs/heads/main/security/goodstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Nonprofits
- Donations
- Charitable Giving
- Fundraising
- Verification
- Compliance
- Payments
- Disbursements
- Social Impact
---
