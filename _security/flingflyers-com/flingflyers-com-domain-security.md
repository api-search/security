---
api_specs:
- filename: flingflyers-com-openapi-generated.yml
  format: yaml
  label: Flyer API
  slug: flingflyers-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flingflyers-com/openapi/_ae-authored/flingflyers-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flingflyers.com
  spf: true
hosts:
- cert_expires: Dec 21 21:34:35 2026 GMT
  host: flingflyers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flyer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flyer
provider_slug: flingflyers-com
slug: flingflyers-com-domain-security
source_filename: flingflyers-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flingflyers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 21:34:35 2026 GMT\n  hsts: false\ndomains:\n- domain: flingflyers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flingflyers-com/security/flingflyers-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
