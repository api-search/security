---
api_specs:
- filename: appmixer-api-openapi.yml
  format: yaml
  label: Appmixer API
  slug: appmixer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appmixer.com
  spf: true
hosts:
- cert_expires: Sep 11 16:17:33 2026 GMT
  host: www.appmixer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 09:04:26 2026 GMT
  host: docs.appmixer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appmixer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appmixer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appmixer
provider_slug: appmixer
slug: appmixer-domain-security
source_filename: appmixer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appmixer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.appmixer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:04:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appmixer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/security/appmixer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
---
