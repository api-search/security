---
api_specs:
- filename: application-platform-openapi-generated.yml
  format: yaml
  label: doppelt.digital API
  slug: application-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-platform/refs/heads/main/openapi/_ae-authored/application-platform-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: application-platform.com
  spf: true
hosts:
- cert_expires: Dec 12 19:37:08 2026 GMT
  host: application-platform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Application Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doppelt.digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: doppelt.digital
provider_slug: application-platform
slug: application-platform-domain-security
source_filename: application-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: application-platform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 19:37:08 2026 GMT\n  hsts: false\ndomains:\n- domain: application-platform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/application-platform/refs/heads/main/security/application-platform-domain-security.yml
summary_line: TLSv1.3
tags:
- Low-code
- Development Platform
- Cloud Hosting
- European SaaS
- Automation
---
