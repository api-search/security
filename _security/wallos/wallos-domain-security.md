---
api_specs:
- filename: wallos-openapi.yml
  format: yaml
  label: Wallos API
  slug: wallos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wallos/openapi/wallos-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wallosapp.com
  spf: false
hosts:
- cert_expires: Jan 17 23:27:28 2027 GMT
  host: wallosapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wallos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wallos
provider_slug: wallos
slug: wallos-domain-security
source_filename: wallos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wallosapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:27:28 2027 GMT\n  hsts: false\ndomains:\n- domain: wallosapp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/wallos/security/wallos-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Subscription
- Finance
- OpenSource
- Tracker
- Personal
---
