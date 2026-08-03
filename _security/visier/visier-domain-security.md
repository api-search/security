---
api_specs:
- filename: visier-administration-apis-openapi.yaml
  format: yaml
  label: Visier Administration APIs
  slug: administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-administration-apis-openapi.yaml
- filename: visier-analytic-model-apis-openapi.yaml
  format: yaml
  label: Visier Analytic Model APIs
  slug: analytic-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-analytic-model-apis-openapi.yaml
- filename: visier-authentication-apis-openapi.yaml
  format: yaml
  label: Visier Authentication APIs
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-authentication-apis-openapi.yaml
- filename: visier-data-in-apis-openapi.yaml
  format: yaml
  label: Visier Data In APIs
  slug: data-in
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-in-apis-openapi.yaml
- filename: visier-data-out-apis-openapi.yaml
  format: yaml
  label: Visier Data Out APIs
  slug: data-out
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-out-apis-openapi.yaml
- filename: visier-webhooks-openapi.yaml
  format: yaml
  label: Visier Webhooks APIs
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-webhooks-openapi.yaml
- filename: visier-planning-openapi.yaml
  format: yaml
  label: Visier Planning Public APIs
  slug: planning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-planning-openapi.yaml
- filename: visier-compensation-benchmarks-openapi.yaml
  format: yaml
  label: Visier Compensation Benchmarks API
  slug: compensation-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-compensation-benchmarks-openapi.yaml
- filename: visier-skills-intelligence-engine-openapi.yaml
  format: yaml
  label: Visier Skills Intelligence Engine API
  slug: skills-intelligence-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-skills-intelligence-engine-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: visier.com
  spf: true
hosts:
- cert_expires: Oct  2 14:23:54 2026 GMT
  host: www.visier.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: docs.visier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Visier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visier, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Visier
provider_slug: visier
slug: visier-domain-security
source_filename: visier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.visier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:23:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.visier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: visier.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/security/visier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- People Analytics
- Workforce Analytics
- Human Resources
- HR Technology
- Workforce Planning
- Analytics
- Business Intelligence
- Compensation
- Skills
- Artificial Intelligence
- Model Context Protocol
---
