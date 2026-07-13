---
api_specs:
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Session (Handshake) API
  slug: bunq-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq User API
  slug: bunq-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Monetary Account API
  slug: bunq-monetary-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Payment API
  slug: bunq-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Request Inquiry API
  slug: bunq-request-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Card API
  slug: bunq-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Attachment API
  slug: bunq-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Customer Statement (Export) API
  slug: bunq-customer-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Notification Filter (Callbacks) API
  slug: bunq-notification-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bunq.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: developer.bunq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 12:03:36 2026 GMT
  host: www.bunq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 11:01:47 2026 GMT
  host: doc.bunq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bunq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bunq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: bunq
provider_slug: bunq
slug: bunq-domain-security
source_filename: bunq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bunq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bunq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.bunq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:01:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bunq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/security/bunq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Neobank
- Payments
- Accounts
- SEPA
- Open Banking
- Fintech
- Europe
- Netherlands
---
