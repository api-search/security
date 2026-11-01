---
api_specs:
- filename: fileflows-openapi-generated.yml
  format: yaml
  label: FileFlows API
  slug: fileflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fileflows/openapi/_ae-authored/fileflows-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fileflows.com
  spf: false
hosts:
- cert_expires: Dec 29 16:44:27 2026 GMT
  host: fileflows.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fileflows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FileFlows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FileFlows
provider_slug: fileflows
slug: fileflows-domain-security
source_filename: fileflows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fileflows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 16:44:27 2026 GMT\n  hsts: false\ndomains:\n- domain: fileflows.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fileflows/security/fileflows-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Automation
- File Processing
- Self-hosted
- Docker
- Open Source
---
