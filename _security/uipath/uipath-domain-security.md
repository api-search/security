---
api_specs:
- filename: uipath-orchestrator-openapi.yml
  format: yaml
  label: UiPath Orchestrator API
  slug: uipath-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-orchestrator-openapi.yml
- filename: uipath-automation-hub-openapi.yml
  format: yaml
  label: UiPath Automation Hub API
  slug: uipath-automation-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-automation-hub-openapi.yml
- filename: uipath-document-understanding-openapi.yml
  format: yaml
  label: UiPath Document Understanding API
  slug: uipath-document-understanding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-document-understanding-openapi.yml
- filename: uipath-data-service-openapi.yml
  format: yaml
  label: UiPath Data Service API
  slug: uipath-data-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-data-service-openapi.yml
- filename: uipath-platform-management-openapi.yml
  format: yaml
  label: UiPath Platform Management API
  slug: uipath-platform-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-platform-management-openapi.yml
- filename: uipath-test-manager-openapi.yml
  format: yaml
  label: UiPath Test Manager API
  slug: uipath-test-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/openapi/uipath-test-manager-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "ssladmin.microsoft.com"
  - 0 issue "web.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uipath.com
  spf: true
hosts:
- cert_expires: Oct  4 09:49:48 2026 GMT
  host: www.uipath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:12:55 2026 GMT
  host: cloud.uipath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 05:16:45 2026 GMT
  host: docs.uipath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uipath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UiPath, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: UiPath
provider_slug: uipath
slug: uipath-domain-security
source_filename: uipath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uipath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:49:48 2026 GMT\n  hsts: false\n- host: cloud.uipath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:12:55 2026 GMT\n  hsts: null\n- host: docs.uipath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:16:45 2026 GMT\n  hsts: null\ndomains:\n- domain: uipath.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"ssladmin.microsoft.com\"\n  - 0 issue \"web.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uipath/refs/heads/main/security/uipath-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Automation
- Robotic Process Automation
- RPA
- Artificial Intelligence
- Document Processing
- Enterprise Automation
- Orchestration
- Testing
---
