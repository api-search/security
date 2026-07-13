---
api_specs:
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Review
  slug: qodo-gen-merge-pr-review-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Code Suggestions
  slug: qodo-gen-merge-code-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge PR Description
  slug: qodo-gen-merge-describe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Merge Ask and Chat
  slug: qodo-gen-merge-ask-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Gen Test Generation
  slug: qodo-gen-test-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
- filename: qodo-gen-openapi.yml
  format: yaml
  label: Qodo Command Agent API
  slug: qodo-gen-command-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/openapi/qodo-gen-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 iodef "mailto:devops@qodo.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qodo.ai
  spf: true
  spf_record: v=spf1 include:_netblocks.google.com include:sendgrid.net include:stspg-customer.com -all
hosts:
- cert_expires: Sep 21 15:24:17 2026 GMT
  host: qodo.ai
  hsts: false
  https: true
  note: Apex 301-redirects to https://www.qodo.ai/; HSTS is set on www, not the apex.
  tls_version: TLSv1.3
- host: www.qodo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.qodo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qodo Gen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qodo
provider_slug: qodo-gen
slug: qodo-gen-domain-security
source_filename: qodo-gen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:24:17 2026 GMT\n  hsts: false\n  note: Apex 301-redirects to https://www.qodo.ai/; HSTS is set on www, not the apex.\n- host: www.qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qodo.ai\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qodo.ai\n  dnssec: false\n  caa:\n  - '0 issue \"godaddy.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"pki.goog; cansignhttpexchanges=yes\"'\n  - '0 issue \"ssl.com\"'\n  - '0 issue \"amazon.com\"'\n  - '0 issue \"comodoca.com\"'\n  - '0 issue \"digicert.com; cansignhttpexchanges=yes\"'\n  - '0 iodef \"mailto:devops@qodo.ai\"'\n  spf: true\n  spf_record: v=spf1 include:_netblocks.google.com include:sendgrid.net include:stspg-customer.com -all\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qodo-gen/refs/heads/main/security/qodo-gen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Coding Assistant
- Code Review
- Test Generation
- Developer Tools
- LLM
- AI
- Pull Request Review
- Code Quality
- Agents
- Open Source
---
