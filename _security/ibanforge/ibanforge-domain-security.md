---
api_specs:
- filename: ibanforge-api-keys-api-openapi.yml
  format: yaml
  label: IBANforge API Keys API
  slug: ibanforge-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-api-keys-api-openapi.yml
- filename: ibanforge-bic-api-openapi.yml
  format: yaml
  label: IBANforge BIC API
  slug: ibanforge-bic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-bic-api-openapi.yml
- filename: ibanforge-compliance-api-openapi.yml
  format: yaml
  label: IBANforge Compliance API
  slug: ibanforge-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-compliance-api-openapi.yml
- filename: ibanforge-credits-api-openapi.yml
  format: yaml
  label: IBANforge Credits API
  slug: ibanforge-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-credits-api-openapi.yml
- filename: ibanforge-free-api-openapi.yml
  format: yaml
  label: IBANforge Free API
  slug: ibanforge-free-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-free-api-openapi.yml
- filename: ibanforge-iban-api-openapi.yml
  format: yaml
  label: IBANforge IBAN API
  slug: ibanforge-iban-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-iban-api-openapi.yml
- filename: ibanforge-mcp-api-openapi.yml
  format: yaml
  label: IBANforge MCP API
  slug: ibanforge-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-mcp-api-openapi.yml
- filename: ibanforge-swiss-clearing-api-openapi.yml
  format: yaml
  label: IBANforge Swiss Clearing API
  slug: ibanforge-swiss-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/openapi/ibanforge-swiss-clearing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ibanforge.com
  spf: true
hosts:
- cert_expires: Aug 30 10:25:02 2026 GMT
  host: api.ibanforge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ibanforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBANforge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IBANforge
provider_slug: ibanforge
slug: ibanforge-domain-security
source_filename: ibanforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.ibanforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ibanforge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibanforge/refs/heads/main/security/ibanforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Banking
- Compliance
- MCP
---
