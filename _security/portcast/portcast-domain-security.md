---
api_specs:
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Container Tracking API
  slug: container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Predictive ETA API
  slug: predictive-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Vessel Schedules API
  slug: vessel-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
- filename: portcast-openapi.yml
  format: yaml
  label: Portcast Webhooks (Push API)
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/openapi/portcast-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: portcast.io
  spf: true
- caa:
  - 0 iodef "mailto:devops@stoplight.io"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Sep 22 02:32:53 2026 GMT
  host: www.portcast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: portcast.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:12:33 2026 GMT
  host: api.portcast.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Portcast
provider_slug: portcast
slug: portcast-domain-security
source_filename: portcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.portcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portcast.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.portcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:12:33 2026 GMT\n  hsts: null\ndomains:\n- domain: portcast.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portcast/refs/heads/main/security/portcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Container Tracking
- Logistics
- Predictive ETA
- Ocean Freight
---
