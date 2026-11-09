---
api_specs:
- filename: amzscout-net-discovery-api-openapi.yml
  format: yaml
  label: AMZScout Discovery API
  slug: amzscout-net-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-discovery-api-openapi.yml
- filename: amzscout-net-dispatch-api-openapi.yml
  format: yaml
  label: AMZScout Dispatch API
  slug: amzscout-net-dispatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-dispatch-api-openapi.yml
- filename: amzscout-net-tools-api-openapi.yml
  format: yaml
  label: AMZScout Tools API
  slug: amzscout-net-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amzscout-net/openapi/amzscout-net-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: amzscout.net
  spf: true
hosts:
- cert_expires: Dec  3 06:36:31 2026 GMT
  host: amzscout.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amzscout Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMZScout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AMZScout
provider_slug: amzscout-net
slug: amzscout-net-domain-security
source_filename: amzscout-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amzscout.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 06:36:31 2026 GMT\n  hsts: false\ndomains:\n- domain: amzscout.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amzscout-net/security/amzscout-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Amazon
- FBA
- Product Research
- Software-as-a-Service
- E-Commerce
- Company
---
