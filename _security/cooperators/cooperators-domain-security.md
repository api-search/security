---
api_specs:
- filename: cooperators-event-insurance-api-openapi.yml
  format: yaml
  label: The Co-operators Event Insurance API
  slug: cooperators-event-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/openapi/cooperators-event-insurance-api-openapi.yml
- filename: cooperators-tenant-insurance-api-openapi.yml
  format: yaml
  label: The Co-operators Tenant Insurance API
  slug: cooperators-tenant-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/openapi/cooperators-tenant-insurance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cooperators.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duuo.ca
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.cooperators.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 11:55:41 2026 GMT
  host: duuo.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cooperators Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Co-operators, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Co-operators
provider_slug: cooperators
slug: cooperators-domain-security
source_filename: cooperators-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cooperators.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n- host: duuo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:55:41 2026 GMT\n  hsts: false\ndomains:\n- domain: cooperators.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: duuo.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooperators/refs/heads/main/security/cooperators-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Canada
- Property and Casualty
- Life Insurance
- Group Benefits
- Embedded Insurance
- Cooperative
- Wealth Management
- Partner API
---
