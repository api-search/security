---
api_specs:
- filename: trustbench-io-receipts-api-openapi.yml
  format: yaml
  label: TrustBench Receipts API
  slug: trustbench-io-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-receipts-api-openapi.yml
- filename: trustbench-io-routing-api-openapi.yml
  format: yaml
  label: TrustBench Routing API
  slug: trustbench-io-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-routing-api-openapi.yml
- filename: trustbench-io-telemetry-api-openapi.yml
  format: yaml
  label: TrustBench Telemetry API
  slug: trustbench-io-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trustbench-io/openapi/trustbench-io-telemetry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: trustbench.io
  spf: false
hosts:
- cert_expires: Jan 28 16:47:27 2027 GMT
  host: trustbench.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TrustBench Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustBench, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TrustBench
provider_slug: trustbench-io
slug: trustbench-io-domain-security
source_filename: trustbench-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustbench.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:47:27 2027 GMT\n  hsts: false\ndomains:\n- domain: trustbench.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trustbench-io/security/trustbench-io-domain-security.yml
summary_line: TLSv1.3
tags:
- FinTech
- Payments
- Blockchain
- Registry
- Telemetry
---
