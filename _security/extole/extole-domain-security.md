---
api_specs:
- filename: extole-integration-consumer-to-extole-openapi.json
  format: json
  label: Extole Integration API - Consumer to Extole
  slug: extole-integration-api-consumer-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-consumer-to-extole-openapi.json
- filename: extole-integration-server-to-extole-openapi.json
  format: json
  label: Extole Integration API - Server to Extole
  slug: extole-integration-api-server-to-extole
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-integration-server-to-extole-openapi.json
- filename: extole-management-openapi.json
  format: json
  label: Extole Management API
  slug: extole-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-openapi.json
- filename: extole-management-expert-openapi.json
  format: json
  label: Extole Management Expert API
  slug: extole-management-expert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/openapi/extole-management-expert-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: extole.com
  spf: true
hosts:
- cert_expires: Aug 19 17:17:54 2026 GMT
  host: extole.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extole, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Extole
provider_slug: extole
slug: extole-domain-security
source_filename: extole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:17:54 2026 GMT\n  hsts: false\ndomains:\n- domain: extole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extole/refs/heads/main/security/extole-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Referral Marketing
- Advocacy
- Loyalty
- Rewards
- Marketing
- Customer Acquisition
- SaaS
---
