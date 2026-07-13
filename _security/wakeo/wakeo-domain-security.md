---
api_specs:
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Shipments API
  slug: wakeo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Tracking API
  slug: wakeo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
- filename: wakeo-openapi.yml
  format: yaml
  label: Wakeo Webhooks API
  slug: wakeo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/openapi/wakeo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:dmarc@wakeo.co
  dnssec: false
  domain: wakeo.co
  spf: true
  spf_record: v=spf1 include:spf.mailjet.com include:_spf.google.com include:mail.zendesk.com include:spf.protection.outlook.com include:26048058.spf06.hubspotemail.net ~all
hosts:
- cert_expires: Sep 23 11:09:53 2026 GMT
  cert_issuer: Let's Encrypt
  host: wakeo.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: Netlify
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  cert_issuer: Amazon
  host: api.wakeo.co
  hsts: false
  https: true
  note: Live production API host. Returns HTTP 403 ForbiddenException (application/json) for unauthenticated requests.
  server: AWS API Gateway
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:44:17 2026 GMT
  cert_issuer: Google Trust Services
  host: docs.wakeo.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Password-protected documentation portal. 302-redirects to /password.
  server: cloudflare
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  cert_issuer: Amazon
  host: app.wakeo.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Web application (S3-hosted SPA).
  server: AmazonS3
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wakeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wakeo, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wakeo
provider_slug: wakeo
slug: wakeo-domain-security
source_filename: wakeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API/docs hosts\nhosts:\n- host: wakeo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 23 11:09:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: Netlify\n- host: api.wakeo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\n  server: AWS API Gateway\n  note: Live production API host. Returns HTTP 403 ForbiddenException (application/json) for unauthenticated requests.\n- host: docs.wakeo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services\n  cert_expires: Oct  9 14:44:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n  note: Password-protected documentation portal. 302-redirects to /password.\n- host: app.wakeo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Amazon\n  cert_expires: Sep 24 23:59:59 2026\
  \ GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: AmazonS3\n  note: Web application (S3-hosted SPA).\ndomains:\n- domain: wakeo.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: \"v=spf1 include:spf.mailjet.com include:_spf.google.com include:mail.zendesk.com include:spf.protection.outlook.com include:26048058.spf06.hubspotemail.net ~all\"\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: \"mailto:dmarc@wakeo.co\"\nnotes: >-\n  All probed Wakeo hosts serve TLS 1.3. The marketing site (wakeo.co) runs on\n  Netlify, the API (api.wakeo.co) on AWS API Gateway, the docs portal\n  (docs.wakeo.co) behind Cloudflare with a password wall, and the app\n  (app.wakeo.co) on Amazon S3. HSTS is present on wakeo.co, docs.wakeo.co, and\n  app.wakeo.co but was not observed on the api.wakeo.co responses. SPF and DMARC\n  (p=quarantine) are configured; DNSSEC was not observed on wakeo.co.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wakeo/refs/heads/main/security/wakeo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Transportation Visibility
- Real-Time Visibility
- Multimodal
- Logistics
- Shipment Tracking
- ETA
- Freight
- Supply Chain Visibility
- SaaS
---
