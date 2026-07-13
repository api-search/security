---
api_specs:
- filename: salesforce-experience-cloud-sites-openapi.yml
  format: yaml
  label: Experience Cloud Sites API
  slug: experience-cloud-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-sites-openapi.yml
- filename: salesforce-experience-cloud-connect-communities-openapi.yml
  format: yaml
  label: Connect REST API (Communities)
  slug: connect-rest-api-communities
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-connect-communities-openapi.yml
- filename: salesforce-experience-cloud-cms-connect-openapi.yml
  format: yaml
  label: CMS Connect API
  slug: cms-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-connect-openapi.yml
- filename: salesforce-experience-cloud-rest-api-openapi.yml
  format: yaml
  label: Salesforce REST API
  slug: salesforce-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-rest-api-openapi.yml
- filename: salesforce-experience-cloud-templates-openapi.yml
  format: yaml
  label: Experience Cloud Templates API
  slug: experience-cloud-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-templates-openapi.yml
- filename: salesforce-experience-cloud-graphql-openapi.yml
  format: yaml
  label: GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-graphql-openapi.yml
- filename: salesforce-experience-cloud-cms-managed-content-openapi.yml
  format: yaml
  label: CMS Managed Content API
  slug: cms-managed-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml
- filename: salesforce-experience-cloud-cms-delivery-openapi.yml
  format: yaml
  label: CMS Delivery API
  slug: cms-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-cms-delivery-openapi.yml
- filename: salesforce-experience-cloud-user-interface-openapi.yml
  format: yaml
  label: User Interface API
  slug: user-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/openapi/salesforce-experience-cloud-user-interface-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.salesforce.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- host: yourinstance.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Experience Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Experience Cloud, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
slug: salesforce-experience-cloud-domain-security
source_filename: salesforce-experience-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: yourinstance.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/security/salesforce-experience-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
---
