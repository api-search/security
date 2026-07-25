---
api_specs:
- filename: instructure-externaltool-api-openapi.yml
  format: yaml
  label: Instructure ExternalTool API
  slug: instructure-externaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-externaltool-api-openapi.yml
- filename: instructure-lti-accountexternaltool-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountExternalTool API
  slug: instructure-lti-accountexternaltool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountexternaltool-api-openapi.yml
- filename: instructure-lti-accountlookup-api-openapi.yml
  format: yaml
  label: Instructure Lti::AccountLookup API
  slug: instructure-lti-accountlookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-accountlookup-api-openapi.yml
- filename: instructure-lti-dataservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::DataService API
  slug: instructure-lti-dataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-dataservice-api-openapi.yml
- filename: instructure-lti-ims-authentication-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Authentication API
  slug: instructure-lti-ims-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-authentication-api-openapi.yml
- filename: instructure-lti-ims-dynamicregistration-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::DynamicRegistration API
  slug: instructure-lti-ims-dynamicregistration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-dynamicregistration-api-openapi.yml
- filename: instructure-lti-ims-lineitem-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::LineItem API
  slug: instructure-lti-ims-lineitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-lineitem-api-openapi.yml
- filename: instructure-lti-ims-namesandrole-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::NamesAndRole API
  slug: instructure-lti-ims-namesandrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-namesandrole-api-openapi.yml
- filename: instructure-lti-ims-result-api-openapi.yml
  format: yaml
  label: Instructure Lti::IMS::Result API
  slug: instructure-lti-ims-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-ims-result-api-openapi.yml
- filename: instructure-lti-membershipservice-api-openapi.yml
  format: yaml
  label: Instructure Lti::MembershipService API
  slug: instructure-lti-membershipservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-membershipservice-api-openapi.yml
- filename: instructure-lti-toolconfigurationsapi-api-openapi.yml
  format: yaml
  label: Instructure Lti::ToolConfigurationsApi API
  slug: instructure-lti-toolconfigurationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-lti-toolconfigurationsapi-api-openapi.yml
- filename: instructure-security-api-openapi.yml
  format: yaml
  label: Instructure Security API
  slug: instructure-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/openapi/instructure-security-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instructure.com
  spf: true
hosts:
- cert_expires: Aug  4 02:52:44 2026 GMT
  host: www.instructure.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 09:17:42 2026 GMT
  host: developerdocs.instructure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api-gateway.instructure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instructure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instructure, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instructure
provider_slug: instructure
slug: instructure-domain-security
source_filename: instructure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 02:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developerdocs.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:17:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gateway.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instructure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instructure/refs/heads/main/security/instructure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EdTech
- Education
- LMS
- Canvas
- Courses
- Enrollments
- Assignments
- Grades
- Discussions
- GraphQL
- LTI
- Learning Management
---
