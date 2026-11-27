---
api_specs:
- filename: leadfast-vip-matches-api-openapi.yml
  format: yaml
  label: LeadFast Matches API
  slug: leadfast-vip-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-matches-api-openapi.yml
- filename: leadfast-vip-monitoring-api-openapi.yml
  format: yaml
  label: LeadFast Monitoring API
  slug: leadfast-vip-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-monitoring-api-openapi.yml
- filename: leadfast-vip-product-api-openapi.yml
  format: yaml
  label: LeadFast Product API
  slug: leadfast-vip-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-product-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadfast.vip
  spf: true
hosts:
- cert_expires: Jan 10 21:15:26 2027 GMT
  host: leadfast.vip
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeadFast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadFast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeadFast
provider_slug: leadfast-vip
slug: leadfast-vip-domain-security
source_filename: leadfast-vip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadfast.vip\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 21:15:26 2027 GMT\n  hsts: false\ndomains:\n- domain: leadfast.vip\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leadfast-vip/security/leadfast-vip-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lead Generation
- Reddit Monitoring
- Software-as-a-Service
- Developer Tools
- Home Automation
- Marketing Automation
---
