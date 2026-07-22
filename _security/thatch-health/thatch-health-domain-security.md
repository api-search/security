---
api_specs:
- filename: thatch-health-platforms-openapi-original.yml
  format: yaml
  label: Thatch for Platforms API
  slug: thatch-for-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-platforms-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thatch.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thatchcloud.com
  spf: true
hosts:
- cert_expires: Oct  3 16:45:17 2026 GMT
  host: thatch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:39:10 2026 GMT
  host: docs.thatch.com
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
name: Thatch Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thatch Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thatch Health
provider_slug: thatch-health
slug: thatch-health-domain-security
source_filename: thatch-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:45:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.thatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:39:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partners.thatchcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:08:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thatchcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/security/thatch-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Benefits
- ICHRA
- Insurance
- Payroll
- Embedded Benefits
- HR
---
