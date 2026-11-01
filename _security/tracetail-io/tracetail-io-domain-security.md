---
api_specs:
- filename: tracetail-io-identification-api-openapi.yml
  format: yaml
  label: tracetail-io Identification API
  slug: tracetail-io-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-identification-api-openapi.yml
- filename: tracetail-io-server-api-api-openapi.yml
  format: yaml
  label: tracetail-io Server API
  slug: tracetail-io-server-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-server-api-api-openapi.yml
- filename: tracetail-io-service-api-openapi.yml
  format: yaml
  label: tracetail-io Service API
  slug: tracetail-io-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-service-api-openapi.yml
- filename: tracetail-io-setup-links-api-openapi.yml
  format: yaml
  label: tracetail-io Setup links API
  slug: tracetail-io-setup-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tracetail-io/openapi/tracetail-io-setup-links-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tracetail.io
  spf: true
hosts:
- cert_expires: Jan 14 09:09:16 2027 GMT
  host: tracetail.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tracetail Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tracetail-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: tracetail-io
provider_slug: tracetail-io
slug: tracetail-io-domain-security
source_filename: tracetail-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tracetail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:09:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tracetail.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tracetail-io/security/tracetail-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Browser Fingerprinting
- Privacy
- Analytics
- API
- Device Identification
---
