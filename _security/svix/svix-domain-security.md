---
api_specs:
- filename: svix-openapi.json
  format: json
  label: Svix Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
- filename: svix-openapi.json
  format: json
  label: Svix Ingest API
  slug: ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
- filename: svix-openapi.json
  format: json
  label: Svix Stream API
  slug: stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/openapi/svix-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: svix.com
  spf: true
hosts:
- cert_expires: Sep 15 00:59:43 2026 GMT
  host: www.svix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.svix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.eu.svix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Svix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Svix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Svix
provider_slug: svix
slug: svix-domain-security
source_filename: svix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.svix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:59:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.svix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eu.svix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: svix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svix/refs/heads/main/security/svix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Webhooks
- Webhooks As A Service
- Webhook Delivery
- Webhook Sending
- Event Driven
- Eventing
- Messaging
- Pub Sub
- Streaming
- Ingest
- Integration
- Reliability
- Retries
- Deliverability
- Signing
- Verification
- HMAC
- Standard Webhooks
- Multi Tenant
- Multi Region
- Enterprise
- SaaS
- Developer Platform
- API
- REST
- SOC 2
- HIPAA
- PCI DSS
- GDPR
- Open Source
- Rust
- Polyglot SDK
- Terraform
- CLI
---
