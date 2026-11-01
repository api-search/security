---
api_specs:
- filename: ontoramp-com-commerce-api-openapi.yml
  format: yaml
  label: ontoramp-com Commerce API
  slug: ontoramp-com-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-commerce-api-openapi.yml
- filename: ontoramp-com-decision-intelligence-api-openapi.yml
  format: yaml
  label: ontoramp-com Decision Intelligence API
  slug: ontoramp-com-decision-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-decision-intelligence-api-openapi.yml
- filename: ontoramp-com-governance-evaluator-api-openapi.yml
  format: yaml
  label: ontoramp-com Governance Evaluator API
  slug: ontoramp-com-governance-evaluator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-governance-evaluator-api-openapi.yml
- filename: ontoramp-com-knowledge-graph-api-openapi.yml
  format: yaml
  label: ontoramp-com Knowledge Graph API
  slug: ontoramp-com-knowledge-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-knowledge-graph-api-openapi.yml
- filename: ontoramp-com-projection-engine-api-openapi.yml
  format: yaml
  label: ontoramp-com Projection Engine API
  slug: ontoramp-com-projection-engine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ontoramp-com/openapi/ontoramp-com-projection-engine-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ontoramp.com
  spf: true
hosts:
- cert_expires: Dec 12 03:12:00 2026 GMT
  host: ontoramp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ontoramp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ontoramp-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ontoramp-com
provider_slug: ontoramp-com
slug: ontoramp-com-domain-security
source_filename: ontoramp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ontoramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 03:12:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ontoramp.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ontoramp-com/security/ontoramp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Governance
- Agentic AI
- Compliance
- Certification
---
