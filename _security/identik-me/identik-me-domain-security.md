---
api_specs:
- filename: identik-me-document-api-openapi.yml
  format: yaml
  label: identik-me Document API
  slug: identik-me-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-api-openapi.yml
- filename: identik-me-document-fields-api-openapi.yml
  format: yaml
  label: identik-me Document Fields API
  slug: identik-me-document-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-fields-api-openapi.yml
- filename: identik-me-document-recipients-api-openapi.yml
  format: yaml
  label: identik-me Document Recipients API
  slug: identik-me-document-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-document-recipients-api-openapi.yml
- filename: identik-me-documents-api-openapi.yml
  format: yaml
  label: identik-me Documents API
  slug: identik-me-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-documents-api-openapi.yml
- filename: identik-me-embedding-api-openapi.yml
  format: yaml
  label: identik-me Embedding API
  slug: identik-me-embedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-embedding-api-openapi.yml
- filename: identik-me-envelope-api-openapi.yml
  format: yaml
  label: identik-me Envelope API
  slug: identik-me-envelope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-api-openapi.yml
- filename: identik-me-envelope-attachments-api-openapi.yml
  format: yaml
  label: identik-me Envelope Attachments API
  slug: identik-me-envelope-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-attachments-api-openapi.yml
- filename: identik-me-envelope-fields-api-openapi.yml
  format: yaml
  label: identik-me Envelope Fields API
  slug: identik-me-envelope-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-fields-api-openapi.yml
- filename: identik-me-envelope-items-api-openapi.yml
  format: yaml
  label: identik-me Envelope Items API
  slug: identik-me-envelope-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-items-api-openapi.yml
- filename: identik-me-envelope-recipients-api-openapi.yml
  format: yaml
  label: identik-me Envelope Recipients API
  slug: identik-me-envelope-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-envelope-recipients-api-openapi.yml
- filename: identik-me-firma-masiva-api-openapi.yml
  format: yaml
  label: identik-me Firma masiva API
  slug: identik-me-firma-masiva-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-firma-masiva-api-openapi.yml
- filename: identik-me-folder-api-openapi.yml
  format: yaml
  label: identik-me Folder API
  slug: identik-me-folder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-folder-api-openapi.yml
- filename: identik-me-representation-api-openapi.yml
  format: yaml
  label: identik-me Representation API
  slug: identik-me-representation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-representation-api-openapi.yml
- filename: identik-me-template-api-openapi.yml
  format: yaml
  label: identik-me Template API
  slug: identik-me-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-api-openapi.yml
- filename: identik-me-template-fields-api-openapi.yml
  format: yaml
  label: identik-me Template Fields API
  slug: identik-me-template-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-fields-api-openapi.yml
- filename: identik-me-template-recipients-api-openapi.yml
  format: yaml
  label: identik-me Template Recipients API
  slug: identik-me-template-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-template-recipients-api-openapi.yml
- filename: identik-me-templates-api-openapi.yml
  format: yaml
  label: identik-me Templates API
  slug: identik-me-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/identik-me/openapi/identik-me-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: identik.me
  spf: true
hosts:
- cert_expires: Dec 27 18:08:22 2026 GMT
  host: identik.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Identik Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for identik-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: identik-me
provider_slug: identik-me
slug: identik-me-domain-security
source_filename: identik-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: identik.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:08:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: identik.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/identik-me/security/identik-me-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DigitalSignature
- DocumentAutomation
- Argentina
- API
---
