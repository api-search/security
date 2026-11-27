---
api_specs:
- filename: amazon-migration-hub-aws-migration-hub-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub AWS Migration Hub API
  slug: amazon-migration-hub-aws-migration-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-aws-migration-hub-api-openapi.yml
- filename: amazon-migration-hub-operations-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Operations API
  slug: amazon-migration-hub-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-operations-api-openapi.yml
- filename: amazon-migration-hub-source-resource-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Source Resource API
  slug: amazon-migration-hub-source-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-source-resource-api-openapi.yml
- filename: amazon-migration-hub-applications-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Applications API
  slug: amazon-migration-hub-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-applications-api-openapi.yml
- filename: amazon-migration-hub-environments-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Environments API
  slug: amazon-migration-hub-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-environments-api-openapi.yml
- filename: amazon-migration-hub-home-region-control-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Home Region Control API
  slug: amazon-migration-hub-home-region-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-home-region-control-api-openapi.yml
- filename: amazon-migration-hub-migrationworkflow-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Migrationworkflow API
  slug: amazon-migration-hub-migrationworkflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-migrationworkflow-api-openapi.yml
- filename: amazon-migration-hub-routes-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Routes API
  slug: amazon-migration-hub-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-routes-api-openapi.yml
- filename: amazon-migration-hub-services-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Services API
  slug: amazon-migration-hub-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-services-api-openapi.yml
- filename: amazon-migration-hub-tags-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Tags API
  slug: amazon-migration-hub-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-tags-api-openapi.yml
- filename: amazon-migration-hub-template-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Template API
  slug: amazon-migration-hub-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-template-api-openapi.yml
- filename: amazon-migration-hub-workflowstep-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Workflowstep API
  slug: amazon-migration-hub-workflowstep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-workflowstep-api-openapi.yml
- filename: amazon-migration-hub-workflowstepgroup-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Migration Hub Workflowstepgroup API
  slug: amazon-migration-hub-workflowstepgroup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-workflowstepgroup-api-openapi.yml
- filename: amazon-migration-hub-resource-policy-api-openapi.yml
  format: yaml
  label: Amazon Migration Hub Resource Policy API
  slug: amazon-migration-hub-resource-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-migration-hub/openapi/amazon-migration-hub-resource-policy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Apr 26 05:01:14 2027 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Migration Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Migration Hub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
slug: amazon-migration-hub-domain-security
source_filename: amazon-migration-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 26 05:01:14 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-migration-hub/security/amazon-migration-hub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Migration
- Cloud Migration
- Cloud
---
