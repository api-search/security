---
api_specs:
- filename: flexim-io-openapi-generated.yml
  format: yaml
  label: Flexim API
  slug: flexim-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flexim-io/openapi/_ae-authored/flexim-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flexim.io
  spf: true
hosts:
- cert_expires: Dec 15 18:31:22 2026 GMT
  host: flexim.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flexim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flexim
provider_slug: flexim-io
slug: flexim-io-domain-security
source_filename: flexim-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 18:31:22 2026 GMT\n  hsts: false\ndomains:\n- domain: flexim.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flexim-io/security/flexim-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEO
- Headless CMS
- Content Automation
- Artificial Intelligence
- Marketing
---
