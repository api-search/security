---
api_specs:
- filename: spektr-openapi.yml
  format: yaml
  label: Spektr API
  slug: spektr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spektr/refs/heads/main/openapi/spektr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spektr.com
  spf: true
hosts:
- cert_expires: Aug 27 05:03:20 2026 GMT
  host: spektr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: ingest.spektr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spektr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spektr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spektr
provider_slug: spektr
slug: spektr-domain-security
source_filename: spektr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spektr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:03:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ingest.spektr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spektr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spektr/refs/heads/main/security/spektr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- RegTech
- KYB
- KYC
- Onboarding
- Transaction Monitoring
- Financial Services
- Artificial Intelligence
- Enterprise
---
