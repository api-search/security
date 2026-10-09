---
api_specs:
- filename: apiaddicts-configuration-api-openapi.yml
  format: yaml
  label: apIAddicts Configuration API
  slug: apiaddicts-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-configuration-api-openapi.yml
- filename: apiaddicts-generator-api-openapi.yml
  format: yaml
  label: apIAddicts Generator API
  slug: apiaddicts-generator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-generator-api-openapi.yml
- filename: apiaddicts-soapui-api-openapi.yml
  format: yaml
  label: apIAddicts Soap UI API
  slug: apiaddicts-soapui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/openapi/apiaddicts-soapui-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiaddicts.org
  spf: true
hosts:
- cert_expires: Nov 30 05:02:46 2026 GMT
  host: www.apiaddicts.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apiaddicts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apIAddicts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: apIAddicts
provider_slug: apiaddicts
slug: apiaddicts-domain-security
source_filename: apiaddicts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiaddicts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 05:02:46 2026 GMT\n  hsts: false\ndomains:\n- domain: apiaddicts.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiaddicts/refs/heads/main/security/apiaddicts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Non-Profit
- Community
- API Training
- Certification
- Events
- Open Source
- API Governance
- Spectral
- MCP
---
