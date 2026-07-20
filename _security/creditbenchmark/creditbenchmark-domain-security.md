---
api_specs:
- filename: creditbenchmark-openapi-original.yml
  format: yaml
  label: Credit Benchmark API
  slug: credit-benchmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/openapi/creditbenchmark-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "starfieldtech.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creditbenchmark.com
  spf: true
hosts:
- cert_expires: Aug  4 10:35:22 2026 GMT
  host: www.creditbenchmark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 10:35:22 2026 GMT
  host: api.creditbenchmark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creditbenchmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit Benchmark, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credit Benchmark
provider_slug: creditbenchmark
slug: creditbenchmark-domain-security
source_filename: creditbenchmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creditbenchmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:35:22 2026 GMT\n  hsts: false\n- host: api.creditbenchmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: creditbenchmark.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creditbenchmark/refs/heads/main/security/creditbenchmark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Risk
- Financial Data
- Credit Ratings
- Analytics
- Risk Management
- Entity Resolution
- Consensus Data
---
