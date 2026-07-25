---
api_specs:
- filename: sysdig-activity-audit-api-openapi.yml
  format: yaml
  label: Sysdig Activity Audit API
  slug: sysdig-activity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-activity-audit-api-openapi.yml
- filename: sysdig-alerts-api-openapi.yml
  format: yaml
  label: Sysdig Alerts API
  slug: sysdig-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-alerts-api-openapi.yml
- filename: sysdig-compliance-api-openapi.yml
  format: yaml
  label: Sysdig Compliance API
  slug: sysdig-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-compliance-api-openapi.yml
- filename: sysdig-dashboards-api-openapi.yml
  format: yaml
  label: Sysdig Dashboards API
  slug: sysdig-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-dashboards-api-openapi.yml
- filename: sysdig-events-api-openapi.yml
  format: yaml
  label: Sysdig Events API
  slug: sysdig-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-events-api-openapi.yml
- filename: sysdig-image-scanning-api-openapi.yml
  format: yaml
  label: Sysdig Image Scanning API
  slug: sysdig-image-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-image-scanning-api-openapi.yml
- filename: sysdig-metrics-api-openapi.yml
  format: yaml
  label: Sysdig Metrics API
  slug: sysdig-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-metrics-api-openapi.yml
- filename: sysdig-notification-channels-api-openapi.yml
  format: yaml
  label: Sysdig Notification Channels API
  slug: sysdig-notification-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-notification-channels-api-openapi.yml
- filename: sysdig-policies-api-openapi.yml
  format: yaml
  label: Sysdig Policies API
  slug: sysdig-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-policies-api-openapi.yml
- filename: sysdig-rules-api-openapi.yml
  format: yaml
  label: Sysdig Rules API
  slug: sysdig-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-rules-api-openapi.yml
- filename: sysdig-sbom-api-openapi.yml
  format: yaml
  label: Sysdig SBOM API
  slug: sysdig-sbom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-sbom-api-openapi.yml
- filename: sysdig-teams-api-openapi.yml
  format: yaml
  label: Sysdig Teams API
  slug: sysdig-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-teams-api-openapi.yml
- filename: sysdig-vulnerabilities-api-openapi.yml
  format: yaml
  label: Sysdig Vulnerabilities API
  slug: sysdig-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-vulnerabilities-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sysdig.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: sysdig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:35:09 2026 GMT
  host: docs.sysdig.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:26:20 2026 GMT
  host: api.us1.sysdig.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sysdig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sysdig, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sysdig
provider_slug: sysdig
slug: sysdig-domain-security
source_filename: sysdig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sysdig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sysdig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us1.sysdig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:26:20 2026 GMT\n  hsts: null\ndomains:\n- domain: sysdig.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/security/sysdig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Containers
- Kubernetes
- Runtime Security
- Security
- Vulnerability Management
- Monitoring
- Observability
- CSPM
- Compliance
---
