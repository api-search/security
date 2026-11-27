---
api_specs:
- filename: nexatron-io-auth-api-openapi.yml
  format: yaml
  label: Nexatron Auth API
  slug: nexatron-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-auth-api-openapi.yml
- filename: nexatron-io-connections-api-openapi.yml
  format: yaml
  label: Nexatron Connections API
  slug: nexatron-io-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-connections-api-openapi.yml
- filename: nexatron-io-contact-api-openapi.yml
  format: yaml
  label: Nexatron Contact API
  slug: nexatron-io-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-contact-api-openapi.yml
- filename: nexatron-io-conversations-api-openapi.yml
  format: yaml
  label: Nexatron Conversations API
  slug: nexatron-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-conversations-api-openapi.yml
- filename: nexatron-io-feedback-api-openapi.yml
  format: yaml
  label: Nexatron Feedback API
  slug: nexatron-io-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-feedback-api-openapi.yml
- filename: nexatron-io-query-api-openapi.yml
  format: yaml
  label: Nexatron Query API
  slug: nexatron-io-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-query-api-openapi.yml
- filename: nexatron-io-semantic-api-openapi.yml
  format: yaml
  label: Nexatron Semantic API
  slug: nexatron-io-semantic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexatron-io/openapi/nexatron-io-semantic-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexatron.io
  spf: true
hosts:
- cert_expires: May 28 05:30:59 2027 GMT
  host: nexatron.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexatron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexatron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexatron
provider_slug: nexatron-io
slug: nexatron-io-domain-security
source_filename: nexatron-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexatron.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 28 05:30:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nexatron.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nexatron-io/security/nexatron-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise
- Context
- Data Integration
---
