---
api_specs:
- filename: postscript-partner-api-openapi.yml
  format: yaml
  label: Postscript Partner API
  slug: postscript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/_original/postscript-partner-api-openapi.yml
- filename: postscript-subscribers-api-openapi.yml
  format: yaml
  label: Postscript Subscribers API
  slug: postscript-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-subscribers-api-openapi.yml
- filename: postscript-events-api-openapi.yml
  format: yaml
  label: Postscript Events API
  slug: postscript-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-events-api-openapi.yml
- filename: postscript-keywords-api-openapi.yml
  format: yaml
  label: Postscript Keywords API
  slug: postscript-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-keywords-api-openapi.yml
- filename: postscript-messages-api-openapi.yml
  format: yaml
  label: Postscript Messages API
  slug: postscript-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-messages-api-openapi.yml
- filename: postscript-webhooks-api-openapi.yml
  format: yaml
  label: Postscript Webhooks API
  slug: postscript-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-webhooks-api-openapi.yml
- filename: postscript-compliance-api-openapi.yml
  format: yaml
  label: Postscript Compliance API
  slug: postscript-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-compliance-api-openapi.yml
- filename: postscript-identity-api-openapi.yml
  format: yaml
  label: Postscript Identity API
  slug: postscript-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-identity-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: postscript.io
  spf: true
hosts:
- cert_expires: Oct 25 13:23:53 2026 GMT
  host: postscript.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:49:26 2026 GMT
  host: developers.postscript.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 09:15:12 2026 GMT
  host: api.postscript.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postscript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postscript, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Postscript
provider_slug: postscript
slug: postscript-domain-security
source_filename: postscript-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postscript.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:23:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.postscript.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:49:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.postscript.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 09:15:12 2026 GMT\n  hsts: false\ndomains:\n- domain: postscript.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/security/postscript-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- Marketing
- Messaging
- E-Commerce
- Shopify
- RCS
- Subscribers
- Webhook
- Compliance
---
