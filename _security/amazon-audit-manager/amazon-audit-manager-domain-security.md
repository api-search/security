---
api_specs:
- filename: amazon-audit-manager-assessments-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Assessments API
  slug: amazon-audit-manager-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-assessments-api-openapi.yml
- filename: amazon-audit-manager-controls-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Controls API
  slug: amazon-audit-manager-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-controls-api-openapi.yml
- filename: amazon-audit-manager-evidence-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Evidence API
  slug: amazon-audit-manager-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-evidence-api-openapi.yml
- filename: amazon-audit-manager-frameworks-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Frameworks API
  slug: amazon-audit-manager-frameworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-frameworks-api-openapi.yml
- filename: amazon-audit-manager-reports-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Reports API
  slug: amazon-audit-manager-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-reports-api-openapi.yml
- filename: amazon-audit-manager-settings-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Settings API
  slug: amazon-audit-manager-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/openapi/amazon-audit-manager-settings-api-openapi.yml
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: auditmanager.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Audit Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Audit Manager, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Audit Manager
provider_slug: amazon-audit-manager
slug: amazon-audit-manager-domain-security
source_filename: amazon-audit-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: auditmanager.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-audit-manager/refs/heads/main/security/amazon-audit-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Audit Manager
- Compliance
- Audit
- Risk Management
---
