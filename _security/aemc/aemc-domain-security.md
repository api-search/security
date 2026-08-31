---
api_specs:
- filename: aemc-glossary-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Glossary API
  slug: aemc-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-glossary-api-openapi.yml
- filename: aemc-rule-content-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Rule Content API
  slug: aemc-rule-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-rule-content-api-openapi.yml
- filename: aemc-rule-versions-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Rule Versions API
  slug: aemc-rule-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-rule-versions-api-openapi.yml
- filename: aemc-search-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Search API
  slug: aemc-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-search-api-openapi.yml
- filename: aemc-settings-api-openapi.yml
  format: yaml
  label: Australian Energy Market Commission Settings API
  slug: aemc-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aemc.gov.au
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.aemc.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: energy-rules.aemc.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aemc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Energy Market Commission, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Australian Energy Market Commission
provider_slug: aemc
slug: aemc-domain-security
source_filename: aemc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aemc.gov.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\n- host: energy-rules.aemc.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aemc.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/security/aemc-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Energy
- Australia
- Energy Markets
- Electricity
- Gas
- Utilities
- Regulations
- Smart Metering
- Consumer Data Right
- Government
- Legal
- Rules
---
