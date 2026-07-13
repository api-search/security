---
api_specs:
- filename: overview
  format: yaml
  label: Commerce Web Services API
  slug: commerce-web-services-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/commerce_web_services/overview
- filename: sap-commerce-cloud-assisted-service-openapi.yml
  format: yaml
  label: Assisted Service Module API
  slug: assisted-service-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-assisted-service-openapi.yml
- filename: sap-commerce-cloud-integration-openapi.yml
  format: yaml
  label: Integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-integration-openapi.yml
- filename: sap-commerce-cloud-admin-openapi.yml
  format: yaml
  label: Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-admin-openapi.yml
- filename: sap-commerce-cloud-product-content-management-openapi.yml
  format: yaml
  label: Product Content Management API
  slug: product-content-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/openapi/sap-commerce-cloud-product-content-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sap Commerce Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Commerce Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
slug: sap-commerce-cloud-domain-security
source_filename: sap-commerce-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/security/sap-commerce-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
---
