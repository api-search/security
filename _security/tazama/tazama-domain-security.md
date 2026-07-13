---
api_specs:
- filename: tazama-transaction-monitoring-service-openapi.yml
  format: yaml
  label: Tazama Transaction Monitoring Service API
  slug: transaction-monitoring-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/openapi/tazama-transaction-monitoring-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tazama.org
  spf: true
hosts:
- cert_expires: Sep  3 06:51:44 2026 GMT
  host: tazama.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tazama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tazama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tazama
provider_slug: tazama
slug: tazama-domain-security
source_filename: tazama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tazama.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 06:51:44 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: tazama.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tazama/refs/heads/main/security/tazama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Technology
- Fraud Detection
- Anti-Money Laundering
- Linux Foundation
- Open Source
- Transaction Monitoring
- ISO 20022
- Real Time
---
