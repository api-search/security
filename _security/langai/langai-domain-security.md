---
api_specs:
- filename: langai-documents-api-openapi.yml
  format: yaml
  label: Lang.ai Documents API
  slug: langai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-documents-api-openapi.yml
- filename: langai-projects-api-openapi.yml
  format: yaml
  label: Lang.ai Projects API
  slug: langai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@lang.ai"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lang.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: lang.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: docs.lang.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: company.lang.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''company.lan'
kind: domain-security
layout: security
method: probed
name: Langai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lang.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lang.ai
provider_slug: langai
slug: langai-domain-security
source_filename: langai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lang.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: docs.lang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: company.lang.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''company.lan'\n  hsts: null\ndomains:\n- domain: lang.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@lang.ai\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/security/langai-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Natural Language Processing
- Conversation Intelligence
- Customer-Support
- Text Classification
- Analytics
- Customer Experience
---
