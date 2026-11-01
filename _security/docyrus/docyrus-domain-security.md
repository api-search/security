---
api_specs:
- filename: docyrus-openapi-generated.yml
  format: yaml
  label: Docyrus, Inc. API
  slug: docyrus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docyrus/openapi/_ae-authored/docyrus-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: docyrus.com
  spf: true
hosts:
- cert_expires: Jan 14 09:35:35 2027 GMT
  host: docyrus.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docyrus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docyrus, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Docyrus, Inc.
provider_slug: docyrus
slug: docyrus-domain-security
source_filename: docyrus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docyrus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:35:35 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: docyrus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/docyrus/security/docyrus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Low-code
- Platform
- Automation
- Enterprise
---
