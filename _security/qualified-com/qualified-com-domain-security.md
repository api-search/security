---
api_specs:
- filename: qualified-com-bot-conversations-api-openapi.yml
  format: yaml
  label: Qualified Bot Conversations API
  slug: qualified-com-bot-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-bot-conversations-api-openapi.yml
- filename: qualified-com-bulk-api-openapi.yml
  format: yaml
  label: Qualified Bulk API
  slug: qualified-com-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-bulk-api-openapi.yml
- filename: qualified-com-cancel-meeting-api-openapi.yml
  format: yaml
  label: Qualified Cancel Meeting API
  slug: qualified-com-cancel-meeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-cancel-meeting-api-openapi.yml
- filename: qualified-com-companies-api-openapi.yml
  format: yaml
  label: Qualified Companies API
  slug: qualified-com-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-companies-api-openapi.yml
- filename: qualified-com-conversations-api-openapi.yml
  format: yaml
  label: Qualified Conversations API
  slug: qualified-com-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-conversations-api-openapi.yml
- filename: qualified-com-emails-api-openapi.yml
  format: yaml
  label: Qualified Emails API
  slug: qualified-com-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-emails-api-openapi.yml
- filename: qualified-com-gdpr-api-openapi.yml
  format: yaml
  label: Qualified GDPR API
  slug: qualified-com-gdpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-gdpr-api-openapi.yml
- filename: qualified-com-leads-api-openapi.yml
  format: yaml
  label: Qualified Leads API
  slug: qualified-com-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-leads-api-openapi.yml
- filename: qualified-com-meetings-api-openapi.yml
  format: yaml
  label: Qualified Meetings API
  slug: qualified-com-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-meetings-api-openapi.yml
- filename: qualified-com-messages-api-openapi.yml
  format: yaml
  label: Qualified Messages API
  slug: qualified-com-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-messages-api-openapi.yml
- filename: qualified-com-rep-conversations-api-openapi.yml
  format: yaml
  label: Qualified Rep Conversations API
  slug: qualified-com-rep-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-rep-conversations-api-openapi.yml
- filename: qualified-com-sessions-api-openapi.yml
  format: yaml
  label: Qualified Sessions API
  slug: qualified-com-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qualified.com
  spf: true
hosts:
- cert_expires: Nov 12 13:45:55 2026 GMT
  host: www.qualified.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 13:45:55 2026 GMT
  host: api.qualified.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualified Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualified, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qualified
provider_slug: qualified-com
slug: qualified-com-domain-security
source_filename: qualified-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qualified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:45:55 2026 GMT\n  hsts: false\n- host: api.qualified.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:45:55 2026 GMT\n  hsts: null\ndomains:\n- domain: qualified.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/security/qualified-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversational Marketing
- Sales
- Marketing
- Artificial Intelligence
- AI Agents
- Lead Generation
- Customer Engagement
- Salesforce
- Analytics
---
