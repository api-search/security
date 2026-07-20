---
api_specs:
- filename: aito-technologies-openapi-original.yml
  format: yaml
  label: Aito.ai Query API
  slug: aitoai-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aito-technologies/refs/heads/main/openapi/aito-technologies-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aito.ai
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: aito.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: shared.aito.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aito Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aito Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aito Technologies
provider_slug: aito-technologies
slug: aito-technologies-domain-security
source_filename: aito-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aito.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\n- host: shared.aito.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: aito.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aito-technologies/refs/heads/main/security/aito-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Predictive Database
- Machine Learning
- Artificial Intelligence
- Recommendations
- Search
- Predictive Analytics
- Automation
- Data
---
