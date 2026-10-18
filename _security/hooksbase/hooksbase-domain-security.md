---
api_specs:
- filename: hooksbase-openapi-generated.yml
  format: yaml
  label: Hooksbase API
  slug: hooksbase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooksbase/refs/heads/main/openapi/_ae-authored/hooksbase-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hooksbase.com
  spf: true
hosts:
- cert_expires: Jan 13 07:46:51 2027 GMT
  host: hooksbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hooksbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hooksbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hooksbase
provider_slug: hooksbase
slug: hooksbase-domain-security
source_filename: hooksbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hooksbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 07:46:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hooksbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooksbase/refs/heads/main/security/hooksbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EventInfrastructure
- AI
- Webhooks
- Automation
- Integration
---
