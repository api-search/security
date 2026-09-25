---
api_specs:
- filename: ai-squared-catalogs-api-openapi.yml
  format: yaml
  label: AI Squared Catalogs API
  slug: ai-squared-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-catalogs-api-openapi.yml
- filename: ai-squared-connector-definitions-api-openapi.yml
  format: yaml
  label: AI Squared Connector Definitions API
  slug: ai-squared-connector-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connector-definitions-api-openapi.yml
- filename: ai-squared-connectors-api-openapi.yml
  format: yaml
  label: AI Squared Connectors API
  slug: ai-squared-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-connectors-api-openapi.yml
- filename: ai-squared-models-api-openapi.yml
  format: yaml
  label: AI Squared Models API
  slug: ai-squared-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-models-api-openapi.yml
- filename: ai-squared-syncrecords-api-openapi.yml
  format: yaml
  label: AI Squared Sync Records API
  slug: ai-squared-syncrecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrecords-api-openapi.yml
- filename: ai-squared-syncrun-api-openapi.yml
  format: yaml
  label: AI Squared Sync Run API
  slug: ai-squared-syncrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncrun-api-openapi.yml
- filename: ai-squared-syncruns-api-openapi.yml
  format: yaml
  label: AI Squared Sync Runs API
  slug: ai-squared-syncruns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncruns-api-openapi.yml
- filename: ai-squared-syncs-api-openapi.yml
  format: yaml
  label: AI Squared Syncs API
  slug: ai-squared-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/openapi/ai-squared-syncs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aisquared.ai
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: squared.ai
  spf: true
hosts:
- cert_expires: Nov  8 17:24:43 2026 GMT
  host: aisquared.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 14:44:42 2026 GMT
  host: docs.squared.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 18:37:38 2026 GMT
  host: api.squared.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ai Squared Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Squared, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AI Squared
provider_slug: ai-squared
slug: ai-squared-domain-security
source_filename: ai-squared-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aisquared.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 17:24:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.squared.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 14:44:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.squared.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 18:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aisquared.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: squared.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-squared/refs/heads/main/security/ai-squared-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- Reverse ETL
- Artificial Intelligence
- Machine Learning
- Customer Data Platform
- Data Activation
- Workflow Automation
- Open Source
- MCP
- Enterprise
- A2A
---
