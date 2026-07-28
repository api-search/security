---
api_specs:
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Dispatches API
  slug: voltus-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Sites API
  slug: voltus-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Telemetry API
  slug: voltus-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Webhooks API
  slug: voltus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voltus.co
  spf: true
hosts:
- cert_expires: Oct 14 08:19:52 2026 GMT
  host: www.voltus.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.voltus.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 03:05:05 2026 GMT
  host: openadr.voltus.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voltus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voltus
provider_slug: voltus
slug: voltus-domain-security
source_filename: voltus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voltus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:19:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.voltus.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: openadr.voltus.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 03:05:05 2026 GMT\n  hsts: null\ndomains:\n- domain: voltus.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/security/voltus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Electricity
- Demand Response
- Virtual Power Plant
- DER
- Grid
- Energy Markets
- Flexibility
- Energy Storage
- OpenADR
- Telemetry
---
