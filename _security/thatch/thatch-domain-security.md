---
api_specs:
- filename: thatch-partners-openapi.yml
  format: yaml
  label: Thatch for Platforms API
  slug: thatch-for-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch/refs/heads/main/openapi/thatch-partners-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thatch.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: thatchcloud.com
  spf: true
hosts:
- cert_expires: Sep 25 21:16:30 2026 GMT
  host: thatch.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:08:28 2026 GMT
  host: partners.thatchcloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thatch, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Thatch
provider_slug: thatch
slug: thatch-domain-security
source_filename: thatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thatch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partners.thatchcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:08:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thatch.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thatchcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thatch/refs/heads/main/security/thatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health Insurance
- Health Benefits
- ICHRA
- Employee Benefits
- Payroll
- Insurance
- Fintech
- Embedded Finance
- Company
---
