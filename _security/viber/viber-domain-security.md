---
api_specs:
- filename: viber-account-api-openapi.yml
  format: yaml
  label: Rakuten Viber Account API
  slug: viber-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viber/refs/heads/main/openapi/viber-account-api-openapi.yml
- filename: viber-messages-api-openapi.yml
  format: yaml
  label: Rakuten Viber Messages API
  slug: viber-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viber/refs/heads/main/openapi/viber-messages-api-openapi.yml
- filename: viber-users-api-openapi.yml
  format: yaml
  label: Rakuten Viber Users API
  slug: viber-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viber/refs/heads/main/openapi/viber-users-api-openapi.yml
- filename: viber-webhooks-api-openapi.yml
  format: yaml
  label: Rakuten Viber Webhooks API
  slug: viber-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viber/refs/heads/main/openapi/viber-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viber.com
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: www.viber.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Viber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rakuten Viber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rakuten Viber
provider_slug: viber
slug: viber-domain-security
source_filename: viber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: viber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viber/refs/heads/main/security/viber-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Messaging
- Chatbots
- Communications
---
