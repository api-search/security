---
api_specs:
- filename: myenergi-command-api-openapi.yml
  format: yaml
  label: myenergi Command API
  slug: myenergi-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-command-api-openapi.yml
- filename: myenergi-device-api-openapi.yml
  format: yaml
  label: myenergi Device API
  slug: myenergi-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-device-api-openapi.yml
- filename: myenergi-device-settings-api-openapi.yml
  format: yaml
  label: myenergi Device settings API
  slug: myenergi-device-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-device-settings-api-openapi.yml
- filename: myenergi-devices-api-openapi.yml
  format: yaml
  label: myenergi Devices API
  slug: myenergi-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-devices-api-openapi.yml
- filename: myenergi-gridpay-api-openapi.yml
  format: yaml
  label: myenergi Grid Pay API
  slug: myenergi-gridpay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myenergi/openapi/myenergi-gridpay-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myenergi.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.myenergi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: myenergi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for myenergi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: myenergi
provider_slug: myenergi
slug: myenergi-domain-security
source_filename: myenergi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myenergi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: myenergi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/myenergi/security/myenergi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Renewable Energy
- EV Charging
- Solar
- Battery Storage
---
