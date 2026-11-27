---
api_specs:
- filename: open-factory-com-free-api-openapi.yml
  format: yaml
  label: Open Factory Free API
  slug: open-factory-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-free-api-openapi.yml
- filename: open-factory-com-institutional-api-openapi.yml
  format: yaml
  label: Open Factory Institutional API
  slug: open-factory-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-institutional-api-openapi.yml
- filename: open-factory-com-pro-api-openapi.yml
  format: yaml
  label: Open Factory Pro API
  slug: open-factory-com-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-factory-com/openapi/open-factory-com-pro-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: open-factory.com
  spf: true
hosts:
- cert_expires: Feb 12 11:33:53 2027 GMT
  host: open-factory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Factory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Factory
provider_slug: open-factory-com
slug: open-factory-com-domain-security
source_filename: open-factory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-factory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 11:33:53 2027 GMT\n  hsts: false\ndomains:\n- domain: open-factory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/open-factory-com/security/open-factory-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Research
- Manufacturing
- Data Center
- Equipment
---
