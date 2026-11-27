---
api_specs:
- filename: amazap-com-basics-api-openapi.yml
  format: yaml
  label: Amazap Basics API
  slug: amazap-com-basics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazap-com/openapi/amazap-com-basics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: amazap.com
  spf: true
hosts:
- cert_expires: Jan  7 09:27:26 2027 GMT
  host: amazap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Amazap
provider_slug: amazap-com
slug: amazap-com-domain-security
source_filename: amazap-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amazap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 09:27:26 2027 GMT\n  hsts: false\ndomains:\n- domain: amazap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amazap-com/security/amazap-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Micropayments
- Lightning
- Marketplace
---
