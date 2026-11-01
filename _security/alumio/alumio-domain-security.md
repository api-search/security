---
api_specs:
- filename: alumio-openapi-generated.yml
  format: yaml
  label: Alumio API
  slug: alumio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alumio/openapi/_ae-authored/alumio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alumio.com
  spf: true
hosts:
- cert_expires: Nov 23 04:04:53 2026 GMT
  host: alumio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alumio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alumio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alumio
provider_slug: alumio
slug: alumio-domain-security
source_filename: alumio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alumio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 04:04:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alumio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/alumio/security/alumio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Integration
- iPaaS
- Enterprise
---
