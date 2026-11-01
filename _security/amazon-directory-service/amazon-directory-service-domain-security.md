---
api_specs:
- filename: amazon-directory-service-aws-directory-service-api-openapi.yml
  format: yaml
  label: Amazon Directory Service AWS Directory Service API
  slug: amazon-directory-service-aws-directory-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-aws-directory-service-api-openapi.yml
- filename: amazon-directory-service-ad-assessment-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Ad Assessment API
  slug: amazon-directory-service-ad-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-ad-assessment-api-openapi.yml
- filename: amazon-directory-service-ca-enrollment-policy-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Ca Enrollment Policy API
  slug: amazon-directory-service-ca-enrollment-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-ca-enrollment-policy-api-openapi.yml
- filename: amazon-directory-service-directory-data-access-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Directory Data Access API
  slug: amazon-directory-service-directory-data-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-directory-data-access-api-openapi.yml
- filename: amazon-directory-service-operations-api-openapi.yml
  format: yaml
  label: Amazon Directory Service Directory Service Operations API
  slug: amazon-directory-service-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-directory-service/openapi/amazon-directory-service-operations-api-openapi.yml
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
- host: ds.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Directory Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Directory Service, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
slug: amazon-directory-service-domain-security
source_filename: amazon-directory-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ds.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-directory-service/security/amazon-directory-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Active Directory
- Authentication
- Directory Services
- Identity and Access Management
---
