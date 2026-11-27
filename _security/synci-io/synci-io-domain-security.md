---
api_specs:
- filename: synci-io-openapi-generated.yml
  format: yaml
  label: Synci API
  slug: synci-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synci-io/openapi/_ae-authored/synci-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    agents: []
    checked: '2026-11-25'
    index:
    - alpn:
      - h2
      target: api.synci.io
    published: true
  dnssec: true
  domain: synci.io
  spf: true
hosts:
- cert_expires: Feb 12 18:30:48 2027 GMT
  host: synci.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synci, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Synci
provider_slug: synci-io
slug: synci-io-domain-security
source_filename: synci-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synci.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 18:30:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synci.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: true\n    index:\n    - target: api.synci.io\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/synci-io/security/synci-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- AI
- Finance
- Integration
---
