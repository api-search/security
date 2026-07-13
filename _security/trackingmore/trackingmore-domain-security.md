---
api_specs:
- filename: trackingmore-openapi.yml
  format: yaml
  label: TrackingMore API
  slug: trackingmore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trackingmore/refs/heads/main/openapi/trackingmore-openapi.yml
description: ''
domains:
- caa:
  - www.trackingmore.com.cdn.cloudflare.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: trackingmore.com
  spf: true
hosts:
- cert_expires: Aug 21 19:29:19 2026 GMT
  host: www.trackingmore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 17:06:48 2026 GMT
  host: api.trackingmore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trackingmore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrackingMore, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TrackingMore
provider_slug: trackingmore
slug: trackingmore-domain-security
source_filename: trackingmore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trackingmore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:29:19 2026 GMT\n  hsts: false\n- host: api.trackingmore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:06:48 2026 GMT\n  hsts: false\ndomains:\n- domain: trackingmore.com\n  dnssec: true\n  caa:\n  - www.trackingmore.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trackingmore/refs/heads/main/security/trackingmore-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Logistics
- Shipping
- Tracking
- Parcels
- Webhooks
- Ecommerce
---
