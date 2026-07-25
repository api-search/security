---
api_specs:
- filename: amazon-application-migration-service-applications-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Applications API
  slug: amazon-application-migration-service-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-applications-api-openapi.yml
- filename: amazon-application-migration-service-exports-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Exports API
  slug: amazon-application-migration-service-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-exports-api-openapi.yml
- filename: amazon-application-migration-service-jobs-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Jobs API
  slug: amazon-application-migration-service-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-jobs-api-openapi.yml
- filename: amazon-application-migration-service-launch-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Launch API
  slug: amazon-application-migration-service-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-launch-api-openapi.yml
- filename: amazon-application-migration-service-lifecycle-hooks-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Lifecycle Hooks API
  slug: amazon-application-migration-service-lifecycle-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-lifecycle-hooks-api-openapi.yml
- filename: amazon-application-migration-service-replication-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Replication API
  slug: amazon-application-migration-service-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-replication-api-openapi.yml
- filename: amazon-application-migration-service-source-servers-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Source Servers API
  slug: amazon-application-migration-service-source-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-source-servers-api-openapi.yml
- filename: amazon-application-migration-service-tags-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Tags API
  slug: amazon-application-migration-service-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-tags-api-openapi.yml
- filename: amazon-application-migration-service-vcenter-clients-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Vcenter Clients API
  slug: amazon-application-migration-service-vcenter-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-vcenter-clients-api-openapi.yml
- filename: amazon-application-migration-service-waves-api-openapi.yml
  format: yaml
  label: Amazon Application Migration Service Waves API
  slug: amazon-application-migration-service-waves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/openapi/amazon-application-migration-service-waves-api-openapi.yml
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
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: mgn.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: mgn.eu-west-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Application Migration Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Application Migration Service, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
slug: amazon-application-migration-service-domain-security
source_filename: amazon-application-migration-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: mgn.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\n- host: mgn.eu-west-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/security/amazon-application-migration-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
---
