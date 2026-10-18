---
api_specs:
- filename: foxit-document-generation-api-openapi.yml
  format: yaml
  label: Foxit eSign Document Generation API
  slug: foxit-document-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/openapi/foxit-document-generation-api-openapi.yml
- filename: foxit-documents-api-openapi.yml
  format: yaml
  label: Foxit eSign Documents API
  slug: foxit-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/openapi/foxit-documents-api-openapi.yml
- filename: foxit-foxit-esign-api-api-openapi.yml
  format: yaml
  label: Foxit eSign Foxit ESign API
  slug: foxit-foxit-esign-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/openapi/foxit-foxit-esign-api-api-openapi.yml
- filename: foxit-pdf-services-api-openapi.yml
  format: yaml
  label: Foxit eSign Pdf Services API
  slug: foxit-pdf-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/openapi/foxit-pdf-services-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foxit.com
  spf: true
hosts:
- cert_expires: Feb  2 12:33:51 2027 GMT
  host: foxit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foxit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxit eSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foxit eSign
provider_slug: foxit
slug: foxit-domain-security
source_filename: foxit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 12:33:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: foxit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxit/refs/heads/main/security/foxit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Document Management
- PDF
- Cloud APIs
- Enterprise Software
- Workflow Automation
---
