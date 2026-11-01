---
api_specs:
- filename: amazon-certificate-manager-certificates-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificates API
  slug: amazon-certificate-manager-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-certificates-api-openapi.yml
- filename: amazon-certificate-manager-acme-account-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Account API
  slug: amazon-certificate-manager-acme-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-account-api-openapi.yml
- filename: amazon-certificate-manager-acme-domain-validation-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Domain Validation API
  slug: amazon-certificate-manager-acme-domain-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-domain-validation-api-openapi.yml
- filename: amazon-certificate-manager-acme-endpoint-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme Endpoint API
  slug: amazon-certificate-manager-acme-endpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-endpoint-api-openapi.yml
- filename: amazon-certificate-manager-acme-external-account-binding-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Acme External Account Binding API
  slug: amazon-certificate-manager-acme-external-account-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-acme-external-account-binding-api-openapi.yml
- filename: amazon-certificate-manager-operations-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Operations API
  slug: amazon-certificate-manager-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-operations-api-openapi.yml
- filename: amazon-certificate-manager-tag-api-openapi.yml
  format: yaml
  label: Amazon Certificate Manager Certificate Manager Tag API
  slug: amazon-certificate-manager-tag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-certificate-manager/openapi/amazon-certificate-manager-tag-api-openapi.yml
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
- host: acm.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Certificate Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Certificate Manager, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Certificate Manager
provider_slug: amazon-certificate-manager
slug: amazon-certificate-manager-domain-security
source_filename: amazon-certificate-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: acm.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-certificate-manager/security/amazon-certificate-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Certificates
- Encryption
- Security
- SSL
- TLS
---
