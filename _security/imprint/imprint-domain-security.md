---
api_specs:
- filename: imprint-openapi-original.yml
  format: yaml
  label: Imprint Public API
  slug: imprint-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: imprint.co
  spf: true
hosts:
- cert_expires: Oct  8 22:44:49 2026 GMT
  host: imprint.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:05:19 2026 GMT
  host: dev.sbx.imprint.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imprint, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Imprint
provider_slug: imprint
slug: imprint-domain-security
source_filename: imprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imprint.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:44:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.sbx.imprint.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:05:19 2026 GMT\n  hsts: null\ndomains:\n- domain: imprint.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/security/imprint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Co-Branded Cards
- Payments
- Loans
- Rewards
- Loyalty
- Embedded Finance
---
