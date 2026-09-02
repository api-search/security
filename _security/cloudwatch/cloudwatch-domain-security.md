---
api_specs:
- filename: cloudwatch-alarms-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Alarms API
  slug: cloudwatch-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-alarms-api-openapi.yml
- filename: cloudwatch-anomaly-detection-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Anomaly Detection API
  slug: cloudwatch-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-anomaly-detection-api-openapi.yml
- filename: cloudwatch-composite-alarms-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Composite Alarms API
  slug: cloudwatch-composite-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-composite-alarms-api-openapi.yml
- filename: cloudwatch-dashboards-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Dashboards API
  slug: cloudwatch-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-dashboards-api-openapi.yml
- filename: cloudwatch-metric-streams-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Metric Streams API
  slug: cloudwatch-metric-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-metric-streams-api-openapi.yml
- filename: cloudwatch-metrics-api-openapi.yml
  format: yaml
  label: AWS CloudWatch Metrics API
  slug: cloudwatch-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/openapi/cloudwatch-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: monitoring.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: logs.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cloudwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS CloudWatch, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS CloudWatch
provider_slug: cloudwatch
slug: cloudwatch-domain-security
source_filename: cloudwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: monitoring.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: logs.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/security/cloudwatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alarms
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
---
