---
api_specs:
- filename: mygeocode-openapi-generated.yml
  format: yaml
  label: My Geocode API
  slug: mygeocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mygeocode/openapi/_ae-authored/mygeocode-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mygeocode.com
  spf: true
hosts:
- cert_expires: Feb 10 01:32:52 2027 GMT
  host: mygeocode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: My Geocode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for My Geocode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: My Geocode
provider_slug: mygeocode
slug: mygeocode-domain-security
source_filename: mygeocode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mygeocode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 01:32:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mygeocode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mygeocode/security/mygeocode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- IP Lookup
- Timezone
- Elevation
- Postal Code
---
