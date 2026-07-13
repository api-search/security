---
api_specs:
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Lists API
  slug: emailoctopus-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Contacts API
  slug: emailoctopus-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Campaigns API
  slug: emailoctopus-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Tags API
  slug: emailoctopus-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Automations API
  slug: emailoctopus-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
- filename: emailoctopus-openapi.yml
  format: yaml
  label: EmailOctopus Reports API
  slug: emailoctopus-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/openapi/emailoctopus-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailoctopus.com
  spf: true
hosts:
- cert_expires: Aug 17 15:10:46 2026 GMT
  host: emailoctopus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:44:52 2026 GMT
  host: api.emailoctopus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emailoctopus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailOctopus, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EmailOctopus
provider_slug: emailoctopus
slug: emailoctopus-domain-security
source_filename: emailoctopus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailoctopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.emailoctopus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:44:52 2026 GMT\n  hsts: null\ndomains:\n- domain: emailoctopus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailoctopus/refs/heads/main/security/emailoctopus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Email Marketing
- Newsletters
- Campaigns
- Automation
---
