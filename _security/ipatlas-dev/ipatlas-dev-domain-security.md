---
api_specs:
- filename: ipatlas-dev-openapi-generated.yml
  format: yaml
  label: ipatlas-dev API
  slug: ipatlas-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipatlas-dev/openapi/_ae-authored/ipatlas-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ip-atlas.io
  spf: true
hosts:
- cert_expires: Jan  6 18:34:20 2027 GMT
  host: ip-atlas.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ipatlas Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ipatlas-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ipatlas-dev
provider_slug: ipatlas-dev
slug: ipatlas-dev-domain-security
source_filename: ipatlas-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip-atlas.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:34:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ip-atlas.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ipatlas-dev/security/ipatlas-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IP
- Geolocation
- ASN
- VPN
- Data
---
