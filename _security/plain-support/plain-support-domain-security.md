---
api_specs:
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Customers API
  slug: plain-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Threads API
  slug: plain-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Timeline & Events API
  slug: plain-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Messages API
  slug: plain-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Labels & Tiers API
  slug: plain-labels-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
- filename: plain-support-openapi.yml
  format: yaml
  label: Plain Webhooks API
  slug: plain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/openapi/plain-support-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plain.com
  spf: true
hosts:
- cert_expires: Sep 26 16:49:33 2026 GMT
  host: www.plain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 00:30:43 2026 GMT
  host: core-api.uk.plain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plain Support Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plain, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plain
provider_slug: plain-support
slug: plain-support-domain-security
source_filename: plain-support-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:49:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core-api.uk.plain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:30:43 2026 GMT\n  hsts: null\ndomains:\n- domain: plain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plain-support/refs/heads/main/security/plain-support-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Help Desk
- GraphQL
- Threads
- Customer Communication
- API First
---
