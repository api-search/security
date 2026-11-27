---
api_specs:
- filename: leadstrategist-dk-account-api-openapi.yml
  format: yaml
  label: Lead Strategist Account API
  slug: leadstrategist-dk-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-account-api-openapi.yml
- filename: leadstrategist-dk-companies-api-openapi.yml
  format: yaml
  label: Lead Strategist Companies API
  slug: leadstrategist-dk-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-companies-api-openapi.yml
- filename: leadstrategist-dk-meta-api-openapi.yml
  format: yaml
  label: Lead Strategist Meta API
  slug: leadstrategist-dk-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadstrategist-dk/openapi/leadstrategist-dk-meta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: leadstrategist.dk
  spf: true
hosts:
- cert_expires: Dec 29 13:10:59 2026 GMT
  host: leadstrategist.dk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lead Strategist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Strategist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lead Strategist
provider_slug: leadstrategist-dk
slug: leadstrategist-dk-domain-security
source_filename: leadstrategist-dk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadstrategist.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 13:10:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leadstrategist.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/leadstrategist-dk/security/leadstrategist-dk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Data
- Finance
- Denmark
- CVR
---
