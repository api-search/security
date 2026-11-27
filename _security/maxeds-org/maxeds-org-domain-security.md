---
api_specs:
- filename: maxeds-org-mailbox-api-openapi.yml
  format: yaml
  label: MaxedS Mailbox API
  slug: maxeds-org-mailbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxeds-org/openapi/maxeds-org-mailbox-api-openapi.yml
- filename: maxeds-org-tools-api-openapi.yml
  format: yaml
  label: MaxedS Tools API
  slug: maxeds-org-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxeds-org/openapi/maxeds-org-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maxeds.org
  spf: true
hosts:
- cert_expires: Jan 24 00:02:54 2027 GMT
  host: maxeds.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MaxedS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaxedS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MaxedS
provider_slug: maxeds-org
slug: maxeds-org-domain-security
source_filename: maxeds-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maxeds.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 00:02:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maxeds.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maxeds-org/security/maxeds-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Artificial Intelligence
- Sales
- Automation
- Platform
---
