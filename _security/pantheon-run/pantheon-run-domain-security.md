---
api_specs:
- filename: pantheon-run-ai-api-openapi.yml
  format: yaml
  label: Pantheon AI API
  slug: pantheon-run-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-ai-api-openapi.yml
- filename: pantheon-run-chats-api-openapi.yml
  format: yaml
  label: Pantheon Chats API
  slug: pantheon-run-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-chats-api-openapi.yml
- filename: pantheon-run-contacts-api-openapi.yml
  format: yaml
  label: Pantheon Contacts API
  slug: pantheon-run-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-contacts-api-openapi.yml
- filename: pantheon-run-deals-api-openapi.yml
  format: yaml
  label: Pantheon Deals API
  slug: pantheon-run-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-deals-api-openapi.yml
- filename: pantheon-run-files-api-openapi.yml
  format: yaml
  label: Pantheon Files API
  slug: pantheon-run-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-files-api-openapi.yml
- filename: pantheon-run-r-api-openapi.yml
  format: yaml
  label: Pantheon R API
  slug: pantheon-run-r-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-r-api-openapi.yml
- filename: pantheon-run-records-api-openapi.yml
  format: yaml
  label: Pantheon Records API
  slug: pantheon-run-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-records-api-openapi.yml
- filename: pantheon-run-usage-api-openapi.yml
  format: yaml
  label: Pantheon Usage API
  slug: pantheon-run-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pantheon-run/openapi/pantheon-run-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pantheon.run
  spf: true
hosts:
- cert_expires: Feb  1 02:17:45 2027 GMT
  host: pantheon.run
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pantheon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantheon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pantheon
provider_slug: pantheon-run
slug: pantheon-run-domain-security
source_filename: pantheon-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pantheon.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 02:17:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pantheon.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pantheon-run/security/pantheon-run-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Messaging
- Unified Inbox
- Customer Engagement
- Communications
---
