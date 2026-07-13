---
api_specs:
- filename: mapmyfitness-openapi.yml
  format: yaml
  label: MapMyFitness API
  slug: mapmyfitness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/openapi/mapmyfitness-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: under-armour.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mapmyfitness.com
  spf: true
hosts:
- host: www.under-armour.com
  https: false
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: developer.mapmyfitness.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.ua.com
  https: false
kind: domain-security
layout: security
method: probed
name: Under Armour Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Under Armour, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Under Armour
provider_slug: under-armour
slug: under-armour-domain-security
source_filename: under-armour-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.under-armour.com\n  https: false\n- host: developer.mapmyfitness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.ua.com\n  https: false\ndomains:\n- domain: under-armour.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: mapmyfitness.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/under-armour/refs/heads/main/security/under-armour-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Health
- Wearables
- Connected Fitness
- Sports
- Fortune 1000
---
