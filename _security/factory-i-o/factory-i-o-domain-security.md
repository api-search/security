---
api_specs:
- filename: factory-i-o-web-api.yaml
  format: yaml
  label: FACTORY I/O Web API
  slug: factory-i-o
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/factory-i-o/refs/heads/main/openapi/factory-i-o-web-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: factoryio.com
  spf: true
hosts:
- cert_expires: Aug 24 17:58:06 2026 GMT
  host: factoryio.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 17:58:06 2026 GMT
  host: docs.factoryio.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Factory I O Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FACTORY I/O, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FACTORY I/O
provider_slug: factory-i-o
slug: factory-i-o-domain-security
source_filename: factory-i-o-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factoryio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:58:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.factoryio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:58:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: factoryio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factory-i-o/refs/heads/main/security/factory-i-o-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Industrial Automation
- Simulations
- Software Simulation
---
