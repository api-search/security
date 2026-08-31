---
api_specs:
- filename: mixmax-contact-groups-api-openapi.yml
  format: yaml
  label: Mixmax Contact Groups API
  slug: mixmax-contact-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contact-groups-api-openapi.yml
- filename: mixmax-contacts-api-openapi.yml
  format: yaml
  label: Mixmax Contacts API
  slug: mixmax-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-contacts-api-openapi.yml
- filename: mixmax-file-requests-api-openapi.yml
  format: yaml
  label: Mixmax File Requests API
  slug: mixmax-file-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-file-requests-api-openapi.yml
- filename: mixmax-meetings-api-openapi.yml
  format: yaml
  label: Mixmax Meetings API
  slug: mixmax-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-meetings-api-openapi.yml
- filename: mixmax-sequences-api-openapi.yml
  format: yaml
  label: Mixmax Sequences API
  slug: mixmax-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-sequences-api-openapi.yml
- filename: mixmax-snippet-tags-api-openapi.yml
  format: yaml
  label: Mixmax Snippet Tags API
  slug: mixmax-snippet-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-snippet-tags-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mixmax.com
  spf: true
hosts:
- cert_expires: Sep 28 19:08:31 2026 GMT
  host: www.mixmax.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:35:06 2026 GMT
  host: developer.mixmax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.mixmax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mixmax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mixmax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mixmax
provider_slug: mixmax
slug: mixmax-domain-security
source_filename: mixmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mixmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:08:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.mixmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 19:35:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mixmax.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mixmax.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/security/mixmax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Saas
- MCP
- Agents
- Webhook
- Authentication
- Sales Engagement
- Email
- Sales
- CRM
- Productivity
- Meetings
- Sequences
---
