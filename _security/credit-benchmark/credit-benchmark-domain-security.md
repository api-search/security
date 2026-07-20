---
api_specs:
- filename: credit-benchmark-consensus-data-openapi.yml
  format: yaml
  label: Credit Benchmark Consensus Data API
  slug: credit-benchmark-consensus-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credit-benchmark/refs/heads/main/openapi/credit-benchmark-consensus-data-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "starfieldtech.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creditbenchmark.com
  spf: true
hosts:
- cert_expires: Aug  4 10:35:22 2026 GMT
  host: creditbenchmark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credit Benchmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credit Benchmark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Credit Benchmark
provider_slug: credit-benchmark
slug: credit-benchmark-domain-security
source_filename: credit-benchmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creditbenchmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 10:35:22 2026 GMT\n  hsts: false\ndomains:\n- domain: creditbenchmark.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"starfieldtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credit-benchmark/refs/heads/main/security/credit-benchmark-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Credit Risk
- Credit Ratings
- Financial Data
- Analytics
- Data
- API
---
