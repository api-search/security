---
api_specs:
- filename: mailbuttons-com-auth-api-openapi.yml
  format: yaml
  label: Mailbuttons Auth API
  slug: mailbuttons-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-auth-api-openapi.yml
- filename: mailbuttons-com-jmap-api-openapi.yml
  format: yaml
  label: Mailbuttons Jmap API
  slug: mailbuttons-com-jmap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-jmap-api-openapi.yml
- filename: mailbuttons-com-mailboxes-api-openapi.yml
  format: yaml
  label: Mailbuttons Mailboxes API
  slug: mailbuttons-com-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-mailboxes-api-openapi.yml
- filename: mailbuttons-com-memory-api-openapi.yml
  format: yaml
  label: Mailbuttons Memory API
  slug: mailbuttons-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-memory-api-openapi.yml
- filename: mailbuttons-com-policy-api-openapi.yml
  format: yaml
  label: Mailbuttons Policy API
  slug: mailbuttons-com-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-policy-api-openapi.yml
- filename: mailbuttons-com-send-api-openapi.yml
  format: yaml
  label: Mailbuttons Send API
  slug: mailbuttons-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-send-api-openapi.yml
- filename: mailbuttons-com-threads-api-openapi.yml
  format: yaml
  label: Mailbuttons Threads API
  slug: mailbuttons-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-threads-api-openapi.yml
- filename: mailbuttons-com-webhooks-api-openapi.yml
  format: yaml
  label: Mailbuttons Webhooks API
  slug: mailbuttons-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbuttons-com/openapi/mailbuttons-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailbuttons.com
  spf: true
hosts:
- cert_expires: Jan 18 20:16:32 2027 GMT
  host: mailbuttons.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailbuttons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailbuttons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mailbuttons
provider_slug: mailbuttons-com
slug: mailbuttons-com-domain-security
source_filename: mailbuttons-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailbuttons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 20:16:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mailbuttons.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mailbuttons-com/security/mailbuttons-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Quoting
---
