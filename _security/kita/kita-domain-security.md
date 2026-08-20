---
api_specs:
- filename: kita-applications-api-openapi.yml
  format: yaml
  label: Kita Applications API
  slug: kita-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-applications-api-openapi.yml
- filename: kita-batch-api-openapi.yml
  format: yaml
  label: Kita Batch API
  slug: kita-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-batch-api-openapi.yml
- filename: kita-conversation-api-openapi.yml
  format: yaml
  label: Kita Conversation API
  slug: kita-conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-conversation-api-openapi.yml
- filename: kita-credit-api-openapi.yml
  format: yaml
  label: Kita Credit API
  slug: kita-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-credit-api-openapi.yml
- filename: kita-documents-api-openapi.yml
  format: yaml
  label: Kita Documents API
  slug: kita-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-documents-api-openapi.yml
- filename: kita-exports-api-openapi.yml
  format: yaml
  label: Kita Exports API
  slug: kita-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-exports-api-openapi.yml
- filename: kita-folders-api-openapi.yml
  format: yaml
  label: Kita Folders API
  slug: kita-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-folders-api-openapi.yml
- filename: kita-memo-api-openapi.yml
  format: yaml
  label: Kita Memo API
  slug: kita-memo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-memo-api-openapi.yml
- filename: kita-processing-api-openapi.yml
  format: yaml
  label: Kita Processing API
  slug: kita-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-processing-api-openapi.yml
- filename: kita-results-api-openapi.yml
  format: yaml
  label: Kita Results API
  slug: kita-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-results-api-openapi.yml
- filename: kita-schemas-api-openapi.yml
  format: yaml
  label: Kita Schemas API
  slug: kita-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-schemas-api-openapi.yml
- filename: kita-transcripts-api-openapi.yml
  format: yaml
  label: Kita Transcripts API
  slug: kita-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-transcripts-api-openapi.yml
- filename: kita-verification-api-openapi.yml
  format: yaml
  label: Kita Verification API
  slug: kita-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-verification-api-openapi.yml
- filename: kita-webhooks-api-openapi.yml
  format: yaml
  label: Kita Webhooks API
  slug: kita-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kita.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usekita.com
  spf: true
hosts:
- cert_expires: Aug 24 22:35:38 2026 GMT
  host: www.kita.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:12:47 2026 GMT
  host: portal.usekita.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 05:13:06 2026 GMT
  host: underwriter.kita.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kita Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kita, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kita
provider_slug: kita
slug: kita-domain-security
source_filename: kita-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kita.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:35:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.usekita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: underwriter.kita.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:13:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kita.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: usekita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/security/kita-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Underwriting
- Credit Scoring
- Document Intelligence
- Document Extraction
- Fraud Detection
- Artificial Intelligence
- Computer-Vision
- Emerging Markets
- Loan Origination
---
