---
api_specs:
- filename: sparkpost-dkim-keys-api-openapi.yml
  format: yaml
  label: SparkPost DKIM Keys API
  slug: sparkpost-dkim-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-dkim-keys-api-openapi.yml
- filename: sparkpost-events-api-openapi.yml
  format: yaml
  label: SparkPost Events API
  slug: sparkpost-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-events-api-openapi.yml
- filename: sparkpost-inbound-domains-api-openapi.yml
  format: yaml
  label: SparkPost Inbound Domains API
  slug: sparkpost-inbound-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-inbound-domains-api-openapi.yml
- filename: sparkpost-metrics-api-openapi.yml
  format: yaml
  label: SparkPost Metrics API
  slug: sparkpost-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-metrics-api-openapi.yml
- filename: sparkpost-recipient-lists-api-openapi.yml
  format: yaml
  label: SparkPost Recipient Lists API
  slug: sparkpost-recipient-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-recipient-lists-api-openapi.yml
- filename: sparkpost-relay-webhooks-api-openapi.yml
  format: yaml
  label: SparkPost Relay Webhooks API
  slug: sparkpost-relay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-relay-webhooks-api-openapi.yml
- filename: sparkpost-sending-domains-api-openapi.yml
  format: yaml
  label: SparkPost Sending Domains API
  slug: sparkpost-sending-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-sending-domains-api-openapi.yml
- filename: sparkpost-subaccounts-api-openapi.yml
  format: yaml
  label: SparkPost Subaccounts API
  slug: sparkpost-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-subaccounts-api-openapi.yml
- filename: sparkpost-suppression-list-api-openapi.yml
  format: yaml
  label: SparkPost Suppression List API
  slug: sparkpost-suppression-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-suppression-list-api-openapi.yml
- filename: sparkpost-templates-api-openapi.yml
  format: yaml
  label: SparkPost Templates API
  slug: sparkpost-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-templates-api-openapi.yml
- filename: sparkpost-transmissions-api-openapi.yml
  format: yaml
  label: SparkPost Transmissions API
  slug: sparkpost-transmissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-transmissions-api-openapi.yml
- filename: sparkpost-webhooks-api-openapi.yml
  format: yaml
  label: SparkPost Webhooks API
  slug: sparkpost-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/openapi/sparkpost-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sparkpost.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.sparkpost.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 22:13:51 2026 GMT
  host: developers.sparkpost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.sparkpost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sparkpost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SparkPost, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SparkPost
provider_slug: sparkpost
slug: sparkpost-domain-security
source_filename: sparkpost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sparkpost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.sparkpost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sparkpost.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sparkpost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparkpost/refs/heads/main/security/sparkpost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Transactional Email
- Marketing Email
- Email Delivery
- SMTP
- Webhook
- Analytics
- Templates
- Suppression List
---
