---
api_specs:
- filename: huddlekit-account-api-openapi.yml
  format: yaml
  label: Huddlekit Account API
  slug: huddlekit-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-account-api-openapi.yml
- filename: huddlekit-comments-api-openapi.yml
  format: yaml
  label: Huddlekit Comments API
  slug: huddlekit-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-comments-api-openapi.yml
- filename: huddlekit-events-api-openapi.yml
  format: yaml
  label: Huddlekit Events API
  slug: huddlekit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-events-api-openapi.yml
- filename: huddlekit-projects-api-openapi.yml
  format: yaml
  label: Huddlekit Projects API
  slug: huddlekit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-projects-api-openapi.yml
- filename: huddlekit-webhook-events-api-openapi.yml
  format: yaml
  label: Huddlekit Webhook events API
  slug: huddlekit-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-webhook-events-api-openapi.yml
- filename: huddlekit-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Huddlekit Webhook subscriptions API
  slug: huddlekit-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/openapi/huddlekit-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: huddlekit.com
  spf: true
hosts:
- cert_expires: Nov 19 08:34:13 2026 GMT
  host: huddlekit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Huddlekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huddlekit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Huddlekit
provider_slug: huddlekit
slug: huddlekit-domain-security
source_filename: huddlekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huddlekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:34:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: huddlekit.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huddlekit/refs/heads/main/security/huddlekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Visual Annotation
- Website Feedback
- Developer Tools
- AI Integration
---
