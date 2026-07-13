---
api_specs:
- filename: openapi.json
  format: json
  label: RingCentral Events API
  slug: ringcentral-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ringcentral.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: developer.events.ringcentral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:48:19 2026 GMT
  host: api.events.ringcentral.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RingCentral Events, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RingCentral Events
provider_slug: hopin
slug: hopin-domain-security
source_filename: hopin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.events.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.events.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ringcentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/security/hopin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
---
