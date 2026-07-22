---
api_specs:
- filename: moveworks-events-api-openapi.yaml
  format: yaml
  label: Moveworks Events API
  slug: moveworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-events-api-openapi.yaml
- filename: moveworks-conversations-api-openapi.yaml
  format: yaml
  label: Moveworks Conversations API
  slug: moveworks-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-conversations-api-openapi.yaml
- filename: moveworks-beta-conversations-api-openapi.yaml
  format: yaml
  label: Moveworks Conversations API (Beta)
  slug: moveworks-conversations-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-beta-conversations-api-openapi.yaml
- filename: moveworks-data-api-openapi.yaml
  format: yaml
  label: Moveworks Data API
  slug: moveworks-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-data-api-openapi.yaml
- filename: moveworks-webhook-listeners-openapi.yaml
  format: yaml
  label: Moveworks Webhook Listeners
  slug: moveworks-webhook-listeners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-webhook-listeners-openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:caadns@moveworks.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moveworks.com
  spf: true
- caa:
  - 0 iodef "mailto:caadns@moveworks.ai"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moveworks.ai
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.moveworks.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.moveworks.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.jp.moveworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moveworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moveworks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moveworks
provider_slug: moveworks
slug: moveworks-domain-security
source_filename: moveworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moveworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.moveworks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.jp.moveworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moveworks.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:caadns@moveworks.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moveworks.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caadns@moveworks.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n\
  \  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/security/moveworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agentic AI
- AI Assistant
- Enterprise Automation
- Conversational AI
- Employee Experience
- IT Service Management
- Enterprise Search
---
