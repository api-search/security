---
api_specs:
- filename: amazon-service-catalog-portfolios-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Portfolios API
  slug: amazon-service-catalog-portfolios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-portfolios-api-openapi.yml
- filename: amazon-service-catalog-products-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Products API
  slug: amazon-service-catalog-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-products-api-openapi.yml
- filename: amazon-service-catalog-provisioned-products-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Provisioned Products API
  slug: amazon-service-catalog-provisioned-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioned-products-api-openapi.yml
- filename: amazon-service-catalog-budget-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Budget API
  slug: amazon-service-catalog-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-budget-api-openapi.yml
- filename: amazon-service-catalog-constraint-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Constraint API
  slug: amazon-service-catalog-constraint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-constraint-api-openapi.yml
- filename: amazon-service-catalog-operations-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Operations API
  slug: amazon-service-catalog-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-operations-api-openapi.yml
- filename: amazon-service-catalog-portfolio-share-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Portfolio Share API
  slug: amazon-service-catalog-portfolio-share-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-portfolio-share-api-openapi.yml
- filename: amazon-service-catalog-principal-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Principal API
  slug: amazon-service-catalog-principal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-principal-api-openapi.yml
- filename: amazon-service-catalog-provisioned-product-plan-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Provisioned Product Plan API
  slug: amazon-service-catalog-provisioned-product-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioned-product-plan-api-openapi.yml
- filename: amazon-service-catalog-provisioning-artifact-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Provisioning Artifact API
  slug: amazon-service-catalog-provisioning-artifact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-provisioning-artifact-api-openapi.yml
- filename: amazon-service-catalog-service-action-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Service Action API
  slug: amazon-service-catalog-service-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-service-action-api-openapi.yml
- filename: amazon-service-catalog-tag-option-api-openapi.yml
  format: yaml
  label: Amazon Service Catalog Service Catalog Tag Option API
  slug: amazon-service-catalog-tag-option-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-service-catalog/openapi/amazon-service-catalog-tag-option-api-openapi.yml
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
- host: servicecatalog.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Service Catalog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Service Catalog, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Service Catalog
provider_slug: amazon-service-catalog
slug: amazon-service-catalog-domain-security
source_filename: amazon-service-catalog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: servicecatalog.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-service-catalog/security/amazon-service-catalog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Governance
- Compliance
- IT Governance
- Service Catalog
---
