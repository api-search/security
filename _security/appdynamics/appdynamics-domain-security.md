---
api_specs:
- filename: appdynamics-controller-rest-api-openapi.yml
  format: yaml
  label: AppDynamics Controller REST API
  slug: controller-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-controller-rest-api-openapi.yml
- filename: appdynamics-metric-and-snapshot-api-openapi.yml
  format: yaml
  label: AppDynamics Metric and Snapshot API
  slug: metric-and-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-metric-and-snapshot-api-openapi.yml
- filename: appdynamics-alert-and-respond-api-openapi.yml
  format: yaml
  label: AppDynamics Alert and Respond API
  slug: alert-and-respond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-alert-and-respond-api-openapi.yml
- filename: appdynamics-configuration-api-openapi.yml
  format: yaml
  label: AppDynamics Configuration API
  slug: configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-configuration-api-openapi.yml
- filename: appdynamics-analytics-events-api-openapi.yml
  format: yaml
  label: AppDynamics Analytics Events API
  slug: analytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-analytics-events-api-openapi.yml
- filename: appdynamics-database-agent-api-openapi.yml
  format: yaml
  label: AppDynamics Database Agent API
  slug: database-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-database-agent-api-openapi.yml
- filename: appdynamics-machine-agent-api-openapi.yml
  format: yaml
  label: AppDynamics Machine Agent API
  slug: machine-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-machine-agent-api-openapi.yml
- filename: appdynamics-cloud-observability-api-openapi.yml
  format: yaml
  label: Cisco Cloud Observability API
  slug: cloud-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-cloud-observability-api-openapi.yml
- filename: appdynamics-authentication-api-openapi.yml
  format: yaml
  label: AppDynamics OAuth Authentication API
  slug: authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/openapi/appdynamics-authentication-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@appdynamics.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appdynamics.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 128 issuewild "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 128 iodef "mailto:infosec@cisco.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- host: docs.appdynamics.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Feb 20 00:05:07 2027 GMT
  host: developer.cisco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appdynamics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppDynamics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppDynamics
provider_slug: appdynamics
slug: appdynamics-domain-security
source_filename: appdynamics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.appdynamics.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: developer.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: appdynamics.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@appdynamics.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 128 issuewild \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/security/appdynamics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
---
