---
api_specs:
- filename: etherfax-accounts-api-openapi.yml
  format: yaml
  label: etherFAX Accounts API
  slug: etherfax-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-accounts-api-openapi.yml
- filename: etherfax-devices-api-openapi.yml
  format: yaml
  label: etherFAX Devices API
  slug: etherfax-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-devices-api-openapi.yml
- filename: etherfax-inbox-api-openapi.yml
  format: yaml
  label: etherFAX Inbox API
  slug: etherfax-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-inbox-api-openapi.yml
- filename: etherfax-outbox-api-openapi.yml
  format: yaml
  label: etherFAX Outbox API
  slug: etherfax-outbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-outbox-api-openapi.yml
- filename: etherfax-routes-api-openapi.yml
  format: yaml
  label: etherFAX Routes API
  slug: etherfax-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-routes-api-openapi.yml
- filename: etherfax-status-api-openapi.yml
  format: yaml
  label: etherFAX Status API
  slug: etherfax-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: etherfax.net
  spf: true
hosts:
- cert_expires: Dec 29 15:00:12 2026 GMT
  host: www.etherfax.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Etherfax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for etherFAX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: etherFAX
provider_slug: etherfax
slug: etherfax-domain-security
source_filename: etherfax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.etherfax.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 15:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: etherfax.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/etherfax/security/etherfax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fax
- Cloud
- AI
- Secure
- DocumentAutomation
---
