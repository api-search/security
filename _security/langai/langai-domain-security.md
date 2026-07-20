---
api_specs:
- filename: langai-api-openapi.yml
  format: yaml
  label: Lang.ai API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@lang.ai"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lang.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: lang.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: 'Corrected after the automated probe: lang.ai serves "Strict-Transport-Security: max-age=63072000; includeSubDomains; preload" on its 301 redirect to https://capacity.com/lang/, which the probe followed before reading headers.'
  hsts_preload: true
  https: true
  redirects_to: https://capacity.com/lang/?company=lang.ai
  tls_version: TLSv1.2
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: docs.lang.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: company.lang.ai
  hsts: null
  https: true
  note: Not a real host. "company" is the documented placeholder for a customer's own Lang.ai instance subdomain in the base URL https://{company}.lang.ai/api/v1, so this row is expected to fail verification and is retained only to record that the probe ran.
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''company.lan'
kind: domain-security
layout: security
method: probed
name: Langai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lang.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lang.ai
provider_slug: langai
slug: langai-domain-security
source_filename: langai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lang.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: >-\n    Corrected after the automated probe: lang.ai serves\n    \"Strict-Transport-Security: max-age=63072000; includeSubDomains; preload\" on its 301\n    redirect to https://capacity.com/lang/, which the probe followed before reading\n    headers.\n  redirects_to: https://capacity.com/lang/?company=lang.ai\n- host: docs.lang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: company.lang.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''company.lan'\n  hsts: null\n  note: >-\n    Not a real host. \"company\"\
  \ is the documented placeholder for a customer's own Lang.ai\n    instance subdomain in the base URL https://{company}.lang.ai/api/v1, so this row is\n    expected to fail verification and is retained only to record that the probe ran.\ndomains:\n- domain: lang.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@lang.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/security/langai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Conversation Intelligence
- Customer Support
- Text Classification
- Analytics
- Customer Experience
---
