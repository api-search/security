---
api_specs:
- filename: vs-code-marketplace-gallery-api-openapi.yml
  format: yaml
  label: VS Code Marketplace Gallery API
  slug: vs-code-marketplace-gallery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vs-code-marketplace/refs/heads/main/openapi/vs-code-marketplace-gallery-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: visualstudio.com
  spf: true
hosts:
- cert_expires: Sep  6 13:38:08 2026 GMT
  host: marketplace.visualstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vs Code Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VS Code Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VS Code Marketplace
provider_slug: vs-code-marketplace
slug: vs-code-marketplace-domain-security
source_filename: vs-code-marketplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketplace.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:38:08 2026 GMT\n  hsts: null\ndomains:\n- domain: visualstudio.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vs-code-marketplace/refs/heads/main/security/vs-code-marketplace-domain-security.yml
summary_line: TLSv1.3
tags:
- Developer Tools
- Extensions
- IDE
- Microsoft
---
