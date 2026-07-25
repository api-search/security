---
api_specs:
- filename: sedna-authentication-api-openapi.yml
  format: yaml
  label: SEDNA Authentication API
  slug: sedna-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-authentication-api-openapi.yml
- filename: sedna-category-tag-api-api-openapi.yml
  format: yaml
  label: SEDNA Category Tag API API
  slug: sedna-category-tag-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-category-tag-api-api-openapi.yml
- filename: sedna-comment-api-api-openapi.yml
  format: yaml
  label: SEDNA Comment API API
  slug: sedna-comment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-comment-api-api-openapi.yml
- filename: sedna-company-api-api-openapi.yml
  format: yaml
  label: SEDNA Company API API
  slug: sedna-company-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-company-api-api-openapi.yml
- filename: sedna-contact-api-api-openapi.yml
  format: yaml
  label: SEDNA Contact API API
  slug: sedna-contact-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-contact-api-api-openapi.yml
- filename: sedna-document-api-api-openapi.yml
  format: yaml
  label: SEDNA Document API API
  slug: sedna-document-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-document-api-api-openapi.yml
- filename: sedna-download-api-api-openapi.yml
  format: yaml
  label: SEDNA Download API API
  slug: sedna-download-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-download-api-api-openapi.yml
- filename: sedna-event-api-api-openapi.yml
  format: yaml
  label: SEDNA Event API API
  slug: sedna-event-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-event-api-api-openapi.yml
- filename: sedna-job-reference-api-api-openapi.yml
  format: yaml
  label: SEDNA Job Reference API API
  slug: sedna-job-reference-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-job-reference-api-api-openapi.yml
- filename: sedna-keyword-api-api-openapi.yml
  format: yaml
  label: SEDNA Keyword API API
  slug: sedna-keyword-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-keyword-api-api-openapi.yml
- filename: sedna-message-api-api-openapi.yml
  format: yaml
  label: SEDNA Message API API
  slug: sedna-message-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-message-api-api-openapi.yml
- filename: sedna-saved-search-api-api-openapi.yml
  format: yaml
  label: SEDNA Saved Search API API
  slug: sedna-saved-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-saved-search-api-api-openapi.yml
- filename: sedna-team-api-api-openapi.yml
  format: yaml
  label: SEDNA Team API API
  slug: sedna-team-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-team-api-api-openapi.yml
- filename: sedna-template-api-api-openapi.yml
  format: yaml
  label: SEDNA Template API API
  slug: sedna-template-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-template-api-api-openapi.yml
- filename: sedna-user-api-api-openapi.yml
  format: yaml
  label: SEDNA User API API
  slug: sedna-user-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-user-api-api-openapi.yml
- filename: sedna-vessel-api-api-openapi.yml
  format: yaml
  label: SEDNA Vessel API API
  slug: sedna-vessel-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-vessel-api-api-openapi.yml
- filename: sedna-workflow-api-api-openapi.yml
  format: yaml
  label: SEDNA Workflow API API
  slug: sedna-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-workflow-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sedna.com
  spf: true
hosts:
- cert_expires: Oct  1 05:47:40 2026 GMT
  host: sedna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sedna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEDNA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SEDNA
provider_slug: sedna
slug: sedna-domain-security
source_filename: sedna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sedna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:47:40 2026 GMT\n  hsts: false\ndomains:\n- domain: sedna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/security/sedna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
---
