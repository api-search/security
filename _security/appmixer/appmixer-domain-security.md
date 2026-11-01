---
api_specs:
- filename: appmixer-accounts-api-openapi.yml
  format: yaml
  label: Appmixer Accounts API
  slug: appmixer-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-accounts-api-openapi.yml
- filename: appmixer-apps-api-openapi.yml
  format: yaml
  label: Appmixer Apps API
  slug: appmixer-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-apps-api-openapi.yml
- filename: appmixer-authentication-api-openapi.yml
  format: yaml
  label: Appmixer Authentication API
  slug: appmixer-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-authentication-api-openapi.yml
- filename: appmixer-files-api-openapi.yml
  format: yaml
  label: Appmixer Files API
  slug: appmixer-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-files-api-openapi.yml
- filename: appmixer-flows-api-openapi.yml
  format: yaml
  label: Appmixer Flows API
  slug: appmixer-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-flows-api-openapi.yml
- filename: appmixer-insights-api-openapi.yml
  format: yaml
  label: Appmixer Insights API
  slug: appmixer-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-insights-api-openapi.yml
- filename: appmixer-acl-api-openapi.yml
  format: yaml
  label: Appmixer ACL API
  slug: appmixer-acl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-acl-api-openapi.yml
- filename: appmixer-audit-logs-api-openapi.yml
  format: yaml
  label: Appmixer Audit Logs API
  slug: appmixer-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-audit-logs-api-openapi.yml
- filename: appmixer-automation-hub-api-openapi.yml
  format: yaml
  label: Appmixer Automation Hub API
  slug: appmixer-automation-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-automation-hub-api-openapi.yml
- filename: appmixer-config-api-openapi.yml
  format: yaml
  label: Appmixer Config API
  slug: appmixer-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-config-api-openapi.yml
- filename: appmixer-connector-configuration-api-openapi.yml
  format: yaml
  label: Appmixer Connector Configuration API
  slug: appmixer-connector-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-connector-configuration-api-openapi.yml
- filename: appmixer-integration-categories-api-openapi.yml
  format: yaml
  label: Appmixer Integration Categories API
  slug: appmixer-integration-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-integration-categories-api-openapi.yml
- filename: appmixer-modifiers-api-openapi.yml
  format: yaml
  label: Appmixer Modifiers API
  slug: appmixer-modifiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-modifiers-api-openapi.yml
- filename: appmixer-public-files-api-openapi.yml
  format: yaml
  label: Appmixer Public Files API
  slug: appmixer-public-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-public-files-api-openapi.yml
- filename: appmixer-unprocessed-messages-api-openapi.yml
  format: yaml
  label: Appmixer Unprocessed Messages API
  slug: appmixer-unprocessed-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-unprocessed-messages-api-openapi.yml
- filename: appmixer-user-api-openapi.yml
  format: yaml
  label: Appmixer User API
  slug: appmixer-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-user-api-openapi.yml
- filename: appmixer-user-groups-api-openapi.yml
  format: yaml
  label: Appmixer User Groups API
  slug: appmixer-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-user-groups-api-openapi.yml
- filename: appmixer-variables-api-openapi.yml
  format: yaml
  label: Appmixer Variables API
  slug: appmixer-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-variables-api-openapi.yml
- filename: appmixer-datastores-api-openapi.yml
  format: yaml
  label: Appmixer Datastores API
  slug: appmixer-datastores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmixer/openapi/appmixer-datastores-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appmixer.com
  spf: true
hosts:
- cert_expires: Sep 11 16:17:33 2026 GMT
  host: www.appmixer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 09:04:26 2026 GMT
  host: docs.appmixer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Appmixer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appmixer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appmixer
provider_slug: appmixer
slug: appmixer-domain-security
source_filename: appmixer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appmixer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:17:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.appmixer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:04:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appmixer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/appmixer/security/appmixer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Automation
- Embedded iPaaS
- Integration
- Low-Code
- Workflows
---
