---
api_specs:
- filename: exittaxestimator-com-enquiry-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator Enquiry API
  slug: exittaxestimator-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-enquiry-api-openapi.yml
- filename: exittaxestimator-com-guide-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator Guide API
  slug: exittaxestimator-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-guide-api-openapi.yml
- filename: exittaxestimator-com-mcp-api-openapi.yml
  format: yaml
  label: Exit Tax Estimator MCP API
  slug: exittaxestimator-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exittaxestimator-com/openapi/exittaxestimator-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exittaxestimator.com
  spf: true
hosts:
- cert_expires: Jan 10 11:55:31 2027 GMT
  host: exittaxestimator.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exit Tax Estimator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exit Tax Estimator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exit Tax Estimator
provider_slug: exittaxestimator-com
slug: exittaxestimator-com-domain-security
source_filename: exittaxestimator-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exittaxestimator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:55:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exittaxestimator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/exittaxestimator-com/security/exittaxestimator-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Tax
- Illinois
- ExitTax
- Finance
---
