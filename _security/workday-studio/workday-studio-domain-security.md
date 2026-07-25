---
api_specs:
- filename: workday-studio-absence-management-api-openapi.yml
  format: yaml
  label: Workday Studio Absence Management API
  slug: workday-studio-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-absence-management-api-openapi.yml
- filename: workday-studio-benefits-administration-api-openapi.yml
  format: yaml
  label: Workday Studio Benefits Administration API
  slug: workday-studio-benefits-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-benefits-administration-api-openapi.yml
- filename: workday-studio-compensation-api-openapi.yml
  format: yaml
  label: Workday Studio Compensation API
  slug: workday-studio-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-compensation-api-openapi.yml
- filename: workday-studio-financial-management-api-openapi.yml
  format: yaml
  label: Workday Studio Financial Management API
  slug: workday-studio-financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-financial-management-api-openapi.yml
- filename: workday-studio-human-resources-api-openapi.yml
  format: yaml
  label: Workday Studio Human Resources API
  slug: workday-studio-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-human-resources-api-openapi.yml
- filename: workday-studio-integration-assemblies-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Assemblies API
  slug: workday-studio-integration-assemblies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-assemblies-api-openapi.yml
- filename: workday-studio-integration-events-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Events API
  slug: workday-studio-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-events-api-openapi.yml
- filename: workday-studio-integration-systems-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Systems API
  slug: workday-studio-integration-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-systems-api-openapi.yml
- filename: workday-studio-integration-templates-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Templates API
  slug: workday-studio-integration-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-templates-api-openapi.yml
- filename: workday-studio-launch-parameters-api-openapi.yml
  format: yaml
  label: Workday Studio Launch Parameters API
  slug: workday-studio-launch-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-launch-parameters-api-openapi.yml
- filename: workday-studio-payroll-api-openapi.yml
  format: yaml
  label: Workday Studio Payroll API
  slug: workday-studio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-payroll-api-openapi.yml
- filename: workday-studio-recruiting-api-openapi.yml
  format: yaml
  label: Workday Studio Recruiting API
  slug: workday-studio-recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-recruiting-api-openapi.yml
- filename: workday-studio-service-directory-api-openapi.yml
  format: yaml
  label: Workday Studio Service Directory API
  slug: workday-studio-service-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-service-directory-api-openapi.yml
- filename: workday-studio-staffing-api-openapi.yml
  format: yaml
  label: Workday Studio Staffing API
  slug: workday-studio-staffing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-staffing-api-openapi.yml
- filename: workday-studio-time-tracking-api-openapi.yml
  format: yaml
  label: Workday Studio Time Tracking API
  slug: workday-studio-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-time-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Studio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Studio
provider_slug: workday-studio
slug: workday-studio-domain-security
source_filename: workday-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/security/workday-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Development
- Enterprise
- Finance
- HR
- IDE
- Integration
---
