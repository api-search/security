---
api_specs:
- filename: instapods-openapi-generated.yml
  format: yaml
  label: ExpressTech Systems API
  slug: instapods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapods/refs/heads/main/openapi/_ae-authored/instapods-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: instapods.com
  spf: true
hosts:
- cert_expires: Dec 15 11:04:23 2026 GMT
  host: instapods.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instapods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExpressTech Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ExpressTech Systems
provider_slug: instapods
slug: instapods-domain-security
source_filename: instapods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instapods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 11:04:23 2026 GMT\n  hsts: false\ndomains:\n- domain: instapods.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapods/refs/heads/main/security/instapods-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Deployment
- Cloud
- AI-Integration
- DeveloperTools
---
