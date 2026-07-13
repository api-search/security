---
api_specs:
- filename: loadtestservice.json
  format: json
  label: Azure Load Testing API
  slug: azure-load-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/loadtestservice/resource-manager/Microsoft.LoadTestService/stable/2022-12-01/loadtestservice.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: k6.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grafana.com
  spf: false
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: k6.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: grafana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.k6.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalability Testing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalability Testing, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalability Testing
provider_slug: scalability-testing
slug: scalability-testing-domain-security
source_filename: scalability-testing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: k6.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: grafana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.k6.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: k6.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: grafana.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalability-testing/refs/heads/main/security/scalability-testing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Testing
- Load Testing
- Performance Testing
- Scalability
- Stress Testing
---
