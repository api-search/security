---
api_specs:
- filename: openmail-sh-attachments-api-openapi.yml
  format: yaml
  label: openmail-sh Attachments API
  slug: openmail-sh-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-attachments-api-openapi.yml
- filename: openmail-sh-domains-api-openapi.yml
  format: yaml
  label: openmail-sh Domains API
  slug: openmail-sh-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-domains-api-openapi.yml
- filename: openmail-sh-feedback-api-openapi.yml
  format: yaml
  label: openmail-sh Feedback API
  slug: openmail-sh-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-feedback-api-openapi.yml
- filename: openmail-sh-inboxes-api-openapi.yml
  format: yaml
  label: openmail-sh Inboxes API
  slug: openmail-sh-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-inboxes-api-openapi.yml
- filename: openmail-sh-limits-api-openapi.yml
  format: yaml
  label: openmail-sh Limits API
  slug: openmail-sh-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-limits-api-openapi.yml
- filename: openmail-sh-messages-api-openapi.yml
  format: yaml
  label: openmail-sh Messages API
  slug: openmail-sh-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-messages-api-openapi.yml
- filename: openmail-sh-owned-domains-api-openapi.yml
  format: yaml
  label: openmail-sh Owned Domains API
  slug: openmail-sh-owned-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-owned-domains-api-openapi.yml
- filename: openmail-sh-pods-api-openapi.yml
  format: yaml
  label: openmail-sh Pods API
  slug: openmail-sh-pods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-pods-api-openapi.yml
- filename: openmail-sh-policy-api-openapi.yml
  format: yaml
  label: openmail-sh Policy API
  slug: openmail-sh-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-policy-api-openapi.yml
- filename: openmail-sh-threads-api-openapi.yml
  format: yaml
  label: openmail-sh Threads API
  slug: openmail-sh-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmail-sh/openapi/openmail-sh-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openmail.sh
  spf: true
hosts:
- cert_expires: Nov 28 20:59:21 2026 GMT
  host: openmail.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openmail Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openmail-sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: openmail-sh
provider_slug: openmail-sh
slug: openmail-sh-domain-security
source_filename: openmail-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmail.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 20:59:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openmail.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openmail-sh/security/openmail-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email
- API
- AI
- Developer
---
