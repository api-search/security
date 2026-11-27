---
api_specs:
- filename: amazon-audit-manager-assessments-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Assessments API
  slug: amazon-audit-manager-assessments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-assessments-api-openapi.yml
- filename: amazon-audit-manager-controls-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Controls API
  slug: amazon-audit-manager-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-controls-api-openapi.yml
- filename: amazon-audit-manager-evidence-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Evidence API
  slug: amazon-audit-manager-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-evidence-api-openapi.yml
- filename: amazon-audit-manager-frameworks-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Frameworks API
  slug: amazon-audit-manager-frameworks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-frameworks-api-openapi.yml
- filename: amazon-audit-manager-reports-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Reports API
  slug: amazon-audit-manager-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-reports-api-openapi.yml
- filename: amazon-audit-manager-settings-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Settings API
  slug: amazon-audit-manager-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-settings-api-openapi.yml
- filename: amazon-audit-manager-account-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Account API
  slug: amazon-audit-manager-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-account-api-openapi.yml
- filename: amazon-audit-manager-assessmentframeworksharerequests-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Assessmentframeworksharerequests API
  slug: amazon-audit-manager-assessmentframeworksharerequests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-assessmentframeworksharerequests-api-openapi.yml
- filename: amazon-audit-manager-delegations-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Delegations API
  slug: amazon-audit-manager-delegations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-delegations-api-openapi.yml
- filename: amazon-audit-manager-insights-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Insights API
  slug: amazon-audit-manager-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-insights-api-openapi.yml
- filename: amazon-audit-manager-operations-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Operations API
  slug: amazon-audit-manager-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-operations-api-openapi.yml
- filename: amazon-audit-manager-tags-api-openapi.yml
  format: yaml
  label: Amazon Audit Manager Audit Manager Tags API
  slug: amazon-audit-manager-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-audit-manager/openapi/amazon-audit-manager-tags-api-openapi.yml
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
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 26 05:01:14 2027 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 29 17:29:08 2027 GMT
  host: auditmanager.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon Audit Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Audit Manager, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Audit Manager
provider_slug: amazon-audit-manager
slug: amazon-audit-manager-domain-security
source_filename: amazon-audit-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 26 05:01:14 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: auditmanager.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 17:29:08 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-audit-manager/security/amazon-audit-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Audit Manager
- Compliance
- Audit
- Risk Management
- Amazon Web Services
---
