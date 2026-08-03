---
api_specs:
- filename: tricentis-qtest-manager-openapi.yaml
  format: yaml
  label: qTest Manager API v3
  slug: qtest-manager
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-manager-openapi.yaml
- filename: tricentis-qtest-parameters-openapi.yaml
  format: yaml
  label: qTest Parameters API
  slug: qtest-parameters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-parameters-openapi.yaml
- filename: tricentis-qtest-pulse-openapi.yaml
  format: yaml
  label: qTest Pulse API
  slug: qtest-pulse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-pulse-openapi.yaml
- filename: tricentis-qtest-scenario-openapi.yaml
  format: yaml
  label: qTest Scenario API
  slug: qtest-scenario
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-scenario-openapi.yaml
- filename: tricentis-qtest-sessions-openapi.yaml
  format: yaml
  label: qTest Explorer Sessions API
  slug: qtest-sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-sessions-openapi.yaml
- filename: tricentis-qtest-data-export-openapi.yaml
  format: yaml
  label: qTest Data Export API
  slug: qtest-data-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-data-export-openapi.yaml
- filename: tricentis-qtest-analytics-openapi.json
  format: json
  label: Tricentis Analytics API
  slug: analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-qtest-analytics-openapi.json
- filename: tricentis-neoload-openapi.yaml
  format: yaml
  label: NeoLoad API v3
  slug: neoload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-neoload-openapi.yaml
- filename: tricentis-ttm4j-openapi.json
  format: json
  label: Tricentis Test Management for Jira API
  slug: ttm4j
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/openapi/tricentis-ttm4j-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tricentis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qtestnet.com
  spf: true
hosts:
- cert_expires: Sep 16 13:43:48 2026 GMT
  host: www.tricentis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: docs.tricentis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 22:25:59 2026 GMT
  host: apitryout.qtestnet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tricentis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tricentis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tricentis
provider_slug: tricentis
slug: tricentis-domain-security
source_filename: tricentis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tricentis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tricentis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apitryout.qtestnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 22:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tricentis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: qtestnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tricentis/refs/heads/main/security/tricentis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Testing
- Test Automation
- Quality Engineering
- Test Management
- Performance Testing
- Continuous Testing
- DevOps
- SAP
- Data Integrity
- Agentic Testing
---
