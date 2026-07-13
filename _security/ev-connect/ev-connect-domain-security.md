---
api_specs:
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Stations / Charge Points API
  slug: stations-charge-points
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Connectors API
  slug: connectors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Drivers API
  slug: drivers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Pricing / Plans API
  slug: pricing-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
- filename: ev-connect-openapi.yml
  format: yaml
  label: EV Connect Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/openapi/ev-connect-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evconnect.com
  spf: true
hosts:
- cert_expires: Sep 20 19:49:18 2026 GMT
  host: www.evconnect.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ev Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EV Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EV Connect
provider_slug: ev-connect
slug: ev-connect-domain-security
source_filename: ev-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:49:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: evconnect.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ev-connect/refs/heads/main/security/ev-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EV Charging
- Charge Point Management
- CPMS
- Mobility
- Energy
- OCPP
- OCPI
---
