---
api_specs:
- filename: choreo-api-management-openapi.yml
  format: yaml
  label: Choreo API Management API
  slug: api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-api-management-openapi.yml
- filename: choreo-developer-portal-openapi.yml
  format: yaml
  label: Choreo Developer Portal API
  slug: developer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-developer-portal-openapi.yml
- filename: choreo-insights-openapi.yml
  format: yaml
  label: Choreo Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-insights-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wso2.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: choreo.dev
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: wso2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:58:27 2026 GMT
  host: devportal.choreo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 18:16:21 2026 GMT
  host: console.choreo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Choreo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Choreo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Choreo
provider_slug: choreo
slug: choreo-domain-security
source_filename: choreo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wso2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: devportal.choreo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:58:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.choreo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:16:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wso2.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: choreo.dev\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/security/choreo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
---
