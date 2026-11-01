---
api_specs:
- filename: inflectionio-contact-activity-api-openapi.yml
  format: yaml
  label: Inflection.io Contact Activity API
  slug: inflectionio-contact-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-contact-activity-api-openapi.yml
- filename: inflectionio-contacts-api-openapi.yml
  format: yaml
  label: Inflection.io Contacts API
  slug: inflectionio-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-contacts-api-openapi.yml
- filename: inflectionio-emails-api-openapi.yml
  format: yaml
  label: Inflection.io Emails API
  slug: inflectionio-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-emails-api-openapi.yml
- filename: inflectionio-email-versions-api-openapi.yml
  format: yaml
  label: Inflection.io Email Versions API
  slug: inflectionio-email-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-email-versions-api-openapi.yml
- filename: inflectionio-journeys-api-openapi.yml
  format: yaml
  label: Inflection.io Journeys API
  slug: inflectionio-journeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-journeys-api-openapi.yml
- filename: inflectionio-lists-api-openapi.yml
  format: yaml
  label: Inflection.io Lists API
  slug: inflectionio-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-lists-api-openapi.yml
- filename: inflectionio-organizations-api-openapi.yml
  format: yaml
  label: Inflection.io Organizations API
  slug: inflectionio-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-organizations-api-openapi.yml
- filename: inflectionio-product-users-api-openapi.yml
  format: yaml
  label: Inflection.io Product Users API
  slug: inflectionio-product-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-product-users-api-openapi.yml
- filename: inflectionio-stats-api-openapi.yml
  format: yaml
  label: Inflection.io Stats API
  slug: inflectionio-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflectionio/openapi/inflectionio-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inflection.io
  spf: true
hosts:
- cert_expires: Sep 13 20:35:58 2026 GMT
  host: www.inflection.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.inflection.io
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Inflectionio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflection.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inflection.io
provider_slug: inflectionio
slug: inflectionio-domain-security
source_filename: inflectionio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inflection.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:35:58 2026 GMT\n  hsts: null\n- host: api.inflection.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: inflection.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inflectionio/security/inflectionio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software-as-a-Service
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- MCP
- Agents
- Artificial Intelligence
- Customer Journey
- Webhook
- A2A
---
