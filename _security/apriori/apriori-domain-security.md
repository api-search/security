---
api_specs:
- filename: apriori-agent-api-openapi.yml
  format: yaml
  label: aPriori Agent API
  slug: apriori-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/openapi/apriori-agent-api-openapi.yml
- filename: apriori-workflow-api-openapi.yml
  format: yaml
  label: aPriori Workflow API
  slug: apriori-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/openapi/apriori-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apriori.com
  spf: true
hosts:
- cert_expires: Oct 20 15:49:51 2026 GMT
  host: www.apriori.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 05:04:38 2026 GMT
  host: docs.apriori.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apriori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aPriori, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aPriori
provider_slug: apriori
slug: apriori-domain-security
source_filename: apriori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apriori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 15:49:51 2026 GMT\n  hsts: null\n- host: docs.apriori.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 05:04:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apriori.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/security/apriori-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- manufacturing
- product-cost-management
- design-for-manufacturability
- should-cost
- plm-integration
- cost-engineering
- digital-manufacturing
- sustainability
- workflow-automation
- cad
---
