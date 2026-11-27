---
api_specs:
- filename: testchimp-io-openapi-generated.yml
  format: yaml
  label: TestChimp API
  slug: testchimp-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/testchimp-io/openapi/_ae-authored/testchimp-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: testchimp.io
  spf: true
hosts:
- cert_expires: Jan 28 23:10:56 2027 GMT
  host: testchimp.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TestChimp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TestChimp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TestChimp
provider_slug: testchimp-io
slug: testchimp-io-domain-security
source_filename: testchimp-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: testchimp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:10:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: testchimp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/testchimp-io/security/testchimp-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- QA
- Release Governance
- Agent‑Driven Testing
---
