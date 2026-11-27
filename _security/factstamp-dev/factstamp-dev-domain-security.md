---
api_specs:
- filename: factstamp-dev-api-openapi.json
  format: json
  label: FactStamp Api API
  slug: factstamp-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factstamp-dev/openapi/_original/factstamp-dev-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: factstamp.dev
  spf: true
hosts:
- cert_expires: Jan  8 07:54:39 2027 GMT
  host: factstamp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FactStamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FactStamp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FactStamp
provider_slug: factstamp-dev
slug: factstamp-dev-domain-security
source_filename: factstamp-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factstamp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 07:54:39 2027 GMT\n  hsts: false\ndomains:\n- domain: factstamp.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/factstamp-dev/security/factstamp-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Verification
- Compliance
- Global-Registers
---
