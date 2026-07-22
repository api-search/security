---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sprypoint.com
  spf: true
hosts:
- cert_expires: Sep 18 11:10:03 2026 GMT
  host: sprypoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprypoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpryPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpryPoint
provider_slug: sprypoint
slug: sprypoint-domain-security
source_filename: sprypoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sprypoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sprypoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprypoint/refs/heads/main/security/sprypoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Utilities
- Customer Information System
- Billing
- Payments
- Field Service
- SaaS
---
