---
api_specs:
- filename: rudderstack-gateway-openapi.yml
  format: yaml
  label: RudderStack HTTP Tracking API
  slug: rudderstack-http-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/openapi/rudderstack-gateway-openapi.yml
- filename: rudderstack-event-streaming-asyncapi.yml
  format: yaml
  label: RudderStack Webhook Source API
  slug: rudderstack-webhook-source-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/asyncapi/rudderstack-event-streaming-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rudderstack.com
  spf: true
hosts:
- cert_expires: Aug 13 11:10:43 2026 GMT
  host: www.rudderstack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rudderstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RudderStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RudderStack
provider_slug: rudderstack
slug: rudderstack-domain-security
source_filename: rudderstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rudderstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 11:10:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rudderstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rudderstack/refs/heads/main/security/rudderstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Data Platform
- CDP
- Data Pipeline
- Open Source
- Event Streaming
- Reverse ETL
- Analytics
- Identity Resolution
---
