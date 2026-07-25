---
api_specs:
- filename: aws-security-hub-action-targets-api-openapi.yml
  format: yaml
  label: AWS Security Hub Action Targets API
  slug: aws-security-hub-action-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-action-targets-api-openapi.yml
- filename: aws-security-hub-automation-rules-api-openapi.yml
  format: yaml
  label: AWS Security Hub Automation Rules API
  slug: aws-security-hub-automation-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-automation-rules-api-openapi.yml
- filename: aws-security-hub-configuration-policies-api-openapi.yml
  format: yaml
  label: AWS Security Hub Configuration Policies API
  slug: aws-security-hub-configuration-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-configuration-policies-api-openapi.yml
- filename: aws-security-hub-controls-api-openapi.yml
  format: yaml
  label: AWS Security Hub Controls API
  slug: aws-security-hub-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-controls-api-openapi.yml
- filename: aws-security-hub-findings-api-openapi.yml
  format: yaml
  label: AWS Security Hub Findings API
  slug: aws-security-hub-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-findings-api-openapi.yml
- filename: aws-security-hub-hub-api-openapi.yml
  format: yaml
  label: AWS Security Hub Hub API
  slug: aws-security-hub-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-hub-api-openapi.yml
- filename: aws-security-hub-insights-api-openapi.yml
  format: yaml
  label: AWS Security Hub Insights API
  slug: aws-security-hub-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-insights-api-openapi.yml
- filename: aws-security-hub-invitations-api-openapi.yml
  format: yaml
  label: AWS Security Hub Invitations API
  slug: aws-security-hub-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-invitations-api-openapi.yml
- filename: aws-security-hub-members-api-openapi.yml
  format: yaml
  label: AWS Security Hub Members API
  slug: aws-security-hub-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-members-api-openapi.yml
- filename: aws-security-hub-standards-api-openapi.yml
  format: yaml
  label: AWS Security Hub Standards API
  slug: aws-security-hub-standards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-standards-api-openapi.yml
- filename: aws-security-hub-tags-api-openapi.yml
  format: yaml
  label: AWS Security Hub Tags API
  slug: aws-security-hub-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/openapi/aws-security-hub-tags-api-openapi.yml
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: securityhub.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aws Security Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS Security Hub, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS Security Hub
provider_slug: aws-security-hub
slug: aws-security-hub-domain-security
source_filename: aws-security-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: securityhub.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aws-security-hub/refs/heads/main/security/aws-security-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Cloud Security Posture Management
- Compliance
- Findings
- Threat Detection
- Cloud
---
