---
api_specs:
- filename: 17track-tracking-api-openapi.yml
  format: yaml
  label: 17TRACK Tracking API
  slug: 17track-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/openapi/17track-tracking-api-openapi.yml
- filename: 17track-webhooks-api-openapi.yml
  format: yaml
  label: 17TRACK Webhooks API
  slug: 17track-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/openapi/17track-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 17track.net
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.17track.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.17track.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 17Track Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 17TRACK, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 17TRACK
provider_slug: 17track
slug: 17track-domain-security
source_filename: 17track-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.17track.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\n- host: api.17track.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 17track.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/17track/refs/heads/main/security/17track-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shipping
- Package Tracking
- Logistics
- Carriers
- Delivery
- Webhooks
---
