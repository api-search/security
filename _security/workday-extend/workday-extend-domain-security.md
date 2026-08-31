---
api_specs:
- filename: workday-extend-app-configurations-api-openapi.yml
  format: yaml
  label: Workday Extend App Configurations API
  slug: workday-extend-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-configurations-api-openapi.yml
- filename: workday-extend-app-deployments-api-openapi.yml
  format: yaml
  label: Workday Extend App Deployments API
  slug: workday-extend-app-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-deployments-api-openapi.yml
- filename: workday-extend-app-versions-api-openapi.yml
  format: yaml
  label: Workday Extend App Versions API
  slug: workday-extend-app-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-app-versions-api-openapi.yml
- filename: workday-extend-apps-api-openapi.yml
  format: yaml
  label: Workday Extend Apps API
  slug: workday-extend-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-apps-api-openapi.yml
- filename: workday-extend-custom-object-definitions-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Definitions API
  slug: workday-extend-custom-object-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-definitions-api-openapi.yml
- filename: workday-extend-custom-object-fields-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Fields API
  slug: workday-extend-custom-object-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-fields-api-openapi.yml
- filename: workday-extend-custom-object-instances-api-openapi.yml
  format: yaml
  label: Workday Extend Custom Object Instances API
  slug: workday-extend-custom-object-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-custom-object-instances-api-openapi.yml
- filename: workday-extend-graph-query-api-openapi.yml
  format: yaml
  label: Workday Extend Graph Query API
  slug: workday-extend-graph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-graph-query-api-openapi.yml
- filename: workday-extend-orchestration-executions-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Executions API
  slug: workday-extend-orchestration-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-executions-api-openapi.yml
- filename: workday-extend-orchestration-steps-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Steps API
  slug: workday-extend-orchestration-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-steps-api-openapi.yml
- filename: workday-extend-orchestration-triggers-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestration Triggers API
  slug: workday-extend-orchestration-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestration-triggers-api-openapi.yml
- filename: workday-extend-orchestrations-api-openapi.yml
  format: yaml
  label: Workday Extend Orchestrations API
  slug: workday-extend-orchestrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-orchestrations-api-openapi.yml
- filename: workday-extend-schema-introspection-api-openapi.yml
  format: yaml
  label: Workday Extend Schema Introspection API
  slug: workday-extend-schema-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-schema-introspection-api-openapi.yml
- filename: workday-extend-wql-query-api-openapi.yml
  format: yaml
  label: Workday Extend WQL Query API
  slug: workday-extend-wql-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/openapi/workday-extend-wql-query-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Aug 21 03:09:01 2026 GMT
  host: developer.workday.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: doc.workday.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Extend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Extend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Extend
provider_slug: workday-extend
slug: workday-extend-domain-security
source_filename: workday-extend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-extend/refs/heads/main/security/workday-extend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Custom Applications
- Enterprise
- Extensions
- HCM
- Integration
- Orchestration
- PaaS
---
