---
api_specs:
- filename: quotelinks-openapi-generated.yml
  format: yaml
  label: Quotelinks API
  slug: quotelinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quotelinks/openapi/_ae-authored/quotelinks-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quotelinks.com
  spf: true
hosts:
- cert_expires: Jan 13 19:17:09 2027 GMT
  host: www.quotelinks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quotelinks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quotelinks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quotelinks
provider_slug: quotelinks
slug: quotelinks-domain-security
source_filename: quotelinks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quotelinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:17:09 2027 GMT\n  hsts: false\ndomains:\n- domain: quotelinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/quotelinks/security/quotelinks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Financial Data
- Stocks
- SEC
- Exchange Rates
- Free
- no-api-key
---
