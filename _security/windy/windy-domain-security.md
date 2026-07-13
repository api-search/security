---
api_specs:
- filename: windy-openapi.yml
  format: yaml
  label: Windy Point Forecast API
  slug: point-forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
- filename: windy-openapi.yml
  format: yaml
  label: Windy Map Forecast API
  slug: map-forecast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
- filename: windy-openapi.yml
  format: yaml
  label: Windy Webcams API
  slug: webcams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/openapi/windy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: windy.com
  spf: true
hosts:
- cert_expires: Sep 19 09:31:17 2026 GMT
  host: www.windy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 09:31:17 2026 GMT
  host: api.windy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Windy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Windy
provider_slug: windy
slug: windy-domain-security
source_filename: windy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.windy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:31:17 2026 GMT\n  hsts: false\n- host: api.windy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:31:17 2026 GMT\n  hsts: false\ndomains:\n- domain: windy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windy/refs/heads/main/security/windy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Forecast
- Maps
- Webcams
- Visualization
---
