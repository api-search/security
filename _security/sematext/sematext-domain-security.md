---
api_specs:
- filename: sematext-alert-notifications-api-openapi.yml
  format: yaml
  label: Sematext Alert Notifications API
  slug: sematext-alert-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alert-notifications-api-openapi.yml
- filename: sematext-alerts-api-openapi.yml
  format: yaml
  label: Sematext Alerts API
  slug: sematext-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-alerts-api-openapi.yml
- filename: sematext-app-guests-api-openapi.yml
  format: yaml
  label: Sematext App guests API
  slug: sematext-app-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-guests-api-openapi.yml
- filename: sematext-app-ips-api-openapi.yml
  format: yaml
  label: Sematext App IPs API
  slug: sematext-app-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-ips-api-openapi.yml
- filename: sematext-app-tokens-api-openapi.yml
  format: yaml
  label: Sematext App tokens API
  slug: sematext-app-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-app-tokens-api-openapi.yml
- filename: sematext-apps-api-openapi.yml
  format: yaml
  label: Sematext Apps API
  slug: sematext-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-apps-api-openapi.yml
- filename: sematext-billing-api-openapi.yml
  format: yaml
  label: Sematext Billing API
  slug: sematext-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-billing-api-openapi.yml
- filename: sematext-experience-app-api-openapi.yml
  format: yaml
  label: Sematext Experience App API
  slug: sematext-experience-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-experience-app-api-openapi.yml
- filename: sematext-logs-app-api-openapi.yml
  format: yaml
  label: Sematext Logs App API
  slug: sematext-logs-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-api-openapi.yml
- filename: sematext-logs-app-usage-api-openapi.yml
  format: yaml
  label: Sematext Logs App usage API
  slug: sematext-logs-app-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-logs-app-usage-api-openapi.yml
- filename: sematext-monitoring-app-api-openapi.yml
  format: yaml
  label: Sematext Monitoring App API
  slug: sematext-monitoring-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-monitoring-app-api-openapi.yml
- filename: sematext-notifications-api-openapi.yml
  format: yaml
  label: Sematext Notifications API
  slug: sematext-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-notifications-api-openapi.yml
- filename: sematext-reset-password-api-openapi.yml
  format: yaml
  label: Sematext Reset Password API
  slug: sematext-reset-password-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-reset-password-api-openapi.yml
- filename: sematext-subscriptions-api-openapi.yml
  format: yaml
  label: Sematext Subscriptions API
  slug: sematext-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-subscriptions-api-openapi.yml
- filename: sematext-tags-api-openapi.yml
  format: yaml
  label: Sematext Tags API
  slug: sematext-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/openapi/sematext-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sematext.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: sematext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sematext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sematext, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sematext
provider_slug: sematext
slug: sematext-domain-security
source_filename: sematext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sematext.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sematext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sematext/refs/heads/main/security/sematext-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Observability
- Monitoring
- Logging
- Log Management
- Elasticsearch
- Tracing
- Synthetic Monitoring
- OpenTelemetry
---
