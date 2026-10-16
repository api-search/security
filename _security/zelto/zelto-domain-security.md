---
api_specs:
- filename: zelto-action-checks-api-openapi.yml
  format: yaml
  label: Zelto Action checks API
  slug: zelto-action-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-action-checks-api-openapi.yml
- filename: zelto-agents-api-openapi.yml
  format: yaml
  label: Zelto Agents API
  slug: zelto-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-agents-api-openapi.yml
- filename: zelto-buckets-api-openapi.yml
  format: yaml
  label: Zelto Buckets API
  slug: zelto-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-buckets-api-openapi.yml
- filename: zelto-companies-api-openapi.yml
  format: yaml
  label: Zelto Companies API
  slug: zelto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-companies-api-openapi.yml
- filename: zelto-conversations-api-openapi.yml
  format: yaml
  label: Zelto Conversations API
  slug: zelto-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-conversations-api-openapi.yml
- filename: zelto-customer-metrics-api-openapi.yml
  format: yaml
  label: Zelto Customer Metrics API
  slug: zelto-customer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-customer-metrics-api-openapi.yml
- filename: zelto-experiments-api-openapi.yml
  format: yaml
  label: Zelto Experiments API
  slug: zelto-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-experiments-api-openapi.yml
- filename: zelto-findings-api-openapi.yml
  format: yaml
  label: Zelto Findings API
  slug: zelto-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-findings-api-openapi.yml
- filename: zelto-organizations-api-openapi.yml
  format: yaml
  label: Zelto Organizations API
  slug: zelto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-organizations-api-openapi.yml
- filename: zelto-reports-api-openapi.yml
  format: yaml
  label: Zelto Reports API
  slug: zelto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reports-api-openapi.yml
- filename: zelto-reviews-api-openapi.yml
  format: yaml
  label: Zelto Reviews API
  slug: zelto-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reviews-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@zelto.ai"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zelto.ai
  spf: true
hosts:
- cert_expires: Dec 18 06:24:34 2026 GMT
  host: zelto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zelto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zelto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zelto
provider_slug: zelto
slug: zelto-domain-security
source_filename: zelto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zelto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 06:24:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zelto.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@zelto.ai\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/security/zelto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- VoiceAI
- QA
- Production
- Analytics
- Monitoring
---
