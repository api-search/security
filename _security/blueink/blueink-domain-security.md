---
api_specs:
- filename: blueink-openapi-generated.yml
  format: yaml
  label: BlueInk Technologies API
  slug: blueink-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blueink/openapi/_ae-authored/blueink-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blueink.com
  spf: true
hosts:
- cert_expires: Dec 12 11:29:45 2026 GMT
  host: blueink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blueink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlueInk Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlueInk Technologies
provider_slug: blueink
slug: blueink-domain-security
source_filename: blueink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blueink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 11:29:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blueink.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blueink/security/blueink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSignature
- API
- Government
- Education
- Enterprise
- Compliance
- Workflow
- Integration
---
