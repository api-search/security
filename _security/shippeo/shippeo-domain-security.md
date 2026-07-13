---
api_specs:
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Transport Orders API
  slug: shippeo-transport-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Positions API
  slug: shippeo-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo ETA and Status API
  slug: shippeo-eta-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
- filename: shippeo-openapi.yml
  format: yaml
  label: Shippeo Event Subscriptions (Events-out Webhooks) API
  slug: shippeo-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/openapi/shippeo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 1
  dmarc_policy: quarantine
  dmarc_rua: mailto:webmaster@shippeo.com
  dnssec: false
  domain: shippeo.com
  spf: true
  spf_record: v=spf1 a include:_spf.google.com include:6849930.spf04.hubspotemail.net include:mailgun.org mx ~all
hosts:
- cert_expires: Oct  1 20:46:16 2026 GMT
  cert_subject: developers.shippeo.com
  host: developers.shippeo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: Developer portal (SPA; Redoc/Swagger-based).
  tls_version: TLSv1.3
- cert_expires: Sep 10 12:41:38 2026 GMT
  cert_subject: '*.shippeo.com'
  health_status: 200
  host: api.shippeo.com
  hsts: false
  http_status: 404
  https: true
  note: Production API host, fronted by a Google load balancer. GET /health returns {"http-server":{"healthy":true}}; root returns 404.
  tls_version: TLSv1.3
- cert_expires: Oct  1 07:09:18 2026 GMT
  cert_subject: www.shippeo.com
  host: www.shippeo.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 18:19:05 2026 GMT
  cert_subject: shippeo.com
  host: shippeo.com
  http_status: 301
  https: true
  redirect: https://www.shippeo.com/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shippeo, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shippeo
provider_slug: shippeo
slug: shippeo-domain-security
source_filename: shippeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.shippeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: developers.shippeo.com\n  cert_expires: Oct  1 20:46:16 2026 GMT\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Developer portal (SPA; Redoc/Swagger-based).\n- host: api.shippeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: '*.shippeo.com'\n  cert_expires: Sep 10 12:41:38 2026 GMT\n  http_status: 404\n  health_status: 200\n  hsts: false\n  note: Production API host, fronted by a Google load balancer. GET /health returns {\"http-server\":{\"healthy\":true}}; root returns 404.\n- host: www.shippeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: www.shippeo.com\n  cert_expires: Oct  1 07:09:18 2026 GMT\n  http_status: 200\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n- host:\
  \ shippeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: shippeo.com\n  cert_expires: Sep  6 18:19:05 2026 GMT\n  http_status: 301\n  redirect: https://www.shippeo.com/\ndomains:\n- domain: shippeo.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 a include:_spf.google.com include:6849930.spf04.hubspotemail.net include:mailgun.org mx ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 1\n  dmarc_rua: mailto:webmaster@shippeo.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippeo/refs/heads/main/security/shippeo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Transportation Visibility
- Real-Time Visibility
- Logistics
- Shipment Tracking
- ETA
- Freight
- Supply Chain Visibility
- SaaS
---
