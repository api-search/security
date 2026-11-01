---
api_specs:
- filename: velexa-openapi-generated.yml
  format: yaml
  label: Velexa API
  slug: velexa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/velexa/openapi/_ae-authored/velexa-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: velexa.com
  spf: true
hosts:
- cert_expires: Dec 22 10:29:28 2026 GMT
  host: velexa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Velexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velexa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Velexa
provider_slug: velexa
slug: velexa-domain-security
source_filename: velexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velexa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 10:29:28 2026 GMT\n  hsts: false\ndomains:\n- domain: velexa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/velexa/security/velexa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- WealthTech
- Financial Services
- API Platform
- Institutional Investing
---
