---
api_specs:
- filename: car_configurator
  format: yaml
  label: Mercedes-Benz Car Configurator API
  slug: car-configurator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-benz/refs/heads/main/properties/car_configurator
- filename: command_management_api
  format: yaml
  label: Mercedes-Benz Connect Your Business API
  slug: connect-your-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-benz/refs/heads/main/properties/command_management_api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercedes-benz.com
  spf: true
hosts:
- cert_expires: Aug 24 07:24:23 2026 GMT
  host: developer.mercedes-benz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercedes Benz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercedes-Benz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercedes-Benz
provider_slug: mercedes-benz
slug: mercedes-benz-domain-security
source_filename: mercedes-benz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mercedes-benz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:24:23 2026 GMT\n  hsts: false\ndomains:\n- domain: mercedes-benz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercedes-benz/refs/heads/main/security/mercedes-benz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automobiles
- Cars
- Vehicles
---
