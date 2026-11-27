---
api_specs:
- filename: dottedsign-com-download-api-openapi.yml
  format: yaml
  label: DottedSign Download API
  slug: dottedsign-com-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-download-api-openapi.yml
- filename: dottedsign-com-general-api-openapi.yml
  format: yaml
  label: DottedSign General API
  slug: dottedsign-com-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-general-api-openapi.yml
- filename: dottedsign-com-management-api-openapi.yml
  format: yaml
  label: DottedSign Management API
  slug: dottedsign-com-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-management-api-openapi.yml
- filename: dottedsign-com-seal-api-openapi.yml
  format: yaml
  label: DottedSign Seal API
  slug: dottedsign-com-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-seal-api-openapi.yml
- filename: dottedsign-com-signature-api-openapi.yml
  format: yaml
  label: DottedSign Signature API
  slug: dottedsign-com-signature-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signature-api-openapi.yml
- filename: dottedsign-com-signing-api-openapi.yml
  format: yaml
  label: DottedSign Signing API
  slug: dottedsign-com-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signing-api-openapi.yml
- filename: dottedsign-com-signtask-api-openapi.yml
  format: yaml
  label: DottedSign Sign Task API
  slug: dottedsign-com-signtask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dottedsign-com/openapi/dottedsign-com-signtask-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dottedsign.com
  spf: true
hosts:
- cert_expires: May  3 23:59:59 2027 GMT
  host: dottedsign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DottedSign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DottedSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: DottedSign
provider_slug: dottedsign-com
slug: dottedsign-com-domain-security
source_filename: dottedsign-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dottedsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dottedsign.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dottedsign-com/security/dottedsign-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Signature
- Workflows
- Software-as-a-Service
- Document Management
---
