---
api_specs:
- filename: qualified-com-enterprise-api-openapi.json
  format: json
  label: Qualified Enterprise API
  slug: qualified-com-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-enterprise-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qualified.com
  spf: true
hosts:
- cert_expires: Nov 12 13:45:55 2026 GMT
  host: www.qualified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 13:45:55 2026 GMT
  host: api.qualified.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualified Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualified, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qualified
provider_slug: qualified-com
slug: qualified-com-domain-security
source_filename: qualified-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:45:55 2026 GMT\n  hsts: false\n- host: api.qualified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:45:55 2026 GMT\n  hsts: null\ndomains:\n- domain: qualified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/security/qualified-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversational Marketing
- Sales
- Marketing
- Artificial Intelligence
- AI Agents
- Lead Generation
- Customer Engagement
- Salesforce
- Analytics
---
