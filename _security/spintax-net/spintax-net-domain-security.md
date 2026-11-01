---
api_specs:
- filename: spintax-net-accounts-api-openapi.yml
  format: yaml
  label: spintax-net Accounts API
  slug: spintax-net-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-accounts-api-openapi.yml
- filename: spintax-net-billing-api-openapi.yml
  format: yaml
  label: spintax-net Billing API
  slug: spintax-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-billing-api-openapi.yml
- filename: spintax-net-keys-api-openapi.yml
  format: yaml
  label: spintax-net Keys API
  slug: spintax-net-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-keys-api-openapi.yml
- filename: spintax-net-link-hosts-api-openapi.yml
  format: yaml
  label: spintax-net Link Hosts API
  slug: spintax-net-link-hosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-link-hosts-api-openapi.yml
- filename: spintax-net-links-api-openapi.yml
  format: yaml
  label: spintax-net Links API
  slug: spintax-net-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-links-api-openapi.yml
- filename: spintax-net-me-api-openapi.yml
  format: yaml
  label: spintax-net Me API
  slug: spintax-net-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-me-api-openapi.yml
- filename: spintax-net-partner-api-openapi.yml
  format: yaml
  label: spintax-net Partner API
  slug: spintax-net-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-partner-api-openapi.yml
- filename: spintax-net-sites-api-openapi.yml
  format: yaml
  label: spintax-net Sites API
  slug: spintax-net-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/spintax-net/openapi/spintax-net-sites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: spintax.net
  spf: true
hosts:
- cert_expires: Dec 13 20:27:27 2026 GMT
  host: spintax.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spintax Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for spintax-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: spintax-net
provider_slug: spintax-net
slug: spintax-net-domain-security
source_filename: spintax-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spintax.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 20:27:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spintax.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/spintax-net/security/spintax-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Spintax
- Content Generation
- Template Engine
- Open Source
- API
---
