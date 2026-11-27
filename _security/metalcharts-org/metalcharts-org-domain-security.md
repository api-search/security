---
api_specs:
- filename: metalcharts-org-openapi-generated.yml
  format: yaml
  label: MetalCharts API
  slug: metalcharts-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/metalcharts-org/openapi/_ae-authored/metalcharts-org-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: false
  dnssec: false
  domain: metalcharts.org
  spf: true
hosts:
- cert_expires: Dec 20 21:23:01 2026 GMT
  host: metalcharts.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MetalCharts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetalCharts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MetalCharts
provider_slug: metalcharts-org
slug: metalcharts-org-domain-security
source_filename: metalcharts-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metalcharts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 21:23:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: metalcharts.org\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/metalcharts-org/security/metalcharts-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Metals
- Finance
- Data
- Charts
---
