---
api_specs:
- filename: profound-agents-api-openapi.yml
  format: yaml
  label: Profound Agents API
  slug: profound-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-agents-api-openapi.yml
- filename: profound-beta-api-openapi.yml
  format: yaml
  label: Profound Beta API
  slug: profound-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-beta-api-openapi.yml
- filename: profound-bot-traffic-reports-api-openapi.yml
  format: yaml
  label: Profound Bot Traffic Reports API
  slug: profound-bot-traffic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-bot-traffic-reports-api-openapi.yml
- filename: profound-categories-api-openapi.yml
  format: yaml
  label: Profound Categories API
  slug: profound-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-categories-api-openapi.yml
- filename: profound-content-api-openapi.yml
  format: yaml
  label: Profound Content API
  slug: profound-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-content-api-openapi.yml
- filename: profound-content-optimization-api-openapi.yml
  format: yaml
  label: Profound Content optimization API
  slug: profound-content-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-content-optimization-api-openapi.yml
- filename: profound-documents-api-openapi.yml
  format: yaml
  label: Profound Documents API
  slug: profound-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-documents-api-openapi.yml
- filename: profound-human-referrals-api-openapi.yml
  format: yaml
  label: Profound Human Referrals API
  slug: profound-human-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-human-referrals-api-openapi.yml
- filename: profound-integrations-api-openapi.yml
  format: yaml
  label: Profound Integrations API
  slug: profound-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-integrations-api-openapi.yml
- filename: profound-knowledge-bases-api-openapi.yml
  format: yaml
  label: Profound Knowledge bases API
  slug: profound-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-knowledge-bases-api-openapi.yml
- filename: profound-openai-ads-api-openapi.yml
  format: yaml
  label: Profound OpenAI Ads API
  slug: profound-openai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-openai-ads-api-openapi.yml
- filename: profound-organization-api-openapi.yml
  format: yaml
  label: Profound Organization API
  slug: profound-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-organization-api-openapi.yml
- filename: profound-projects-api-openapi.yml
  format: yaml
  label: Profound Projects API
  slug: profound-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-projects-api-openapi.yml
- filename: profound-prompts-api-openapi.yml
  format: yaml
  label: Profound Prompts API
  slug: profound-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-prompts-api-openapi.yml
- filename: profound-reports-api-openapi.yml
  format: yaml
  label: Profound Reports API
  slug: profound-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-reports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tryprofound.com
  spf: true
hosts:
- cert_expires: Nov  6 05:19:15 2026 GMT
  host: www.tryprofound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 20:14:00 2026 GMT
  host: api.tryprofound.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Profound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Profound, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Profound
provider_slug: profound
slug: profound-domain-security
source_filename: profound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryprofound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 05:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tryprofound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:14:00 2026 GMT\n  hsts: null\ndomains:\n- domain: tryprofound.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/security/profound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Answer Engine Optimization
- AEO
- AI Search
- Generative Engine Optimization
- Marketing
- Analytics
- Agent Analytics
- Brand Visibility
- Citations
- MCP
---
