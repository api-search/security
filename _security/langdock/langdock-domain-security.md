---
api_specs:
- filename: langdock-openapi-original.yml
  format: yaml
  label: Langdock API
  slug: langdock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/openapi/langdock-openapi-original.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@langdock.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: langdock.com
  spf: true
hosts:
- cert_expires: Aug 20 07:00:09 2026 GMT
  host: www.langdock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 21:22:14 2026 GMT
  host: docs.langdock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 15:24:59 2026 GMT
  host: api.langdock.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langdock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Langdock, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Langdock
provider_slug: langdock
slug: langdock-domain-security
source_filename: langdock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.langdock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.langdock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:22:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.langdock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:24:59 2026 GMT\n  hsts: null\ndomains:\n- domain: langdock.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@langdock.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdock/refs/heads/main/security/langdock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise AI
- LLM
- Agents
- Model Context Protocol
- Workflows
- Knowledge Management
- Germany
- Europe
---
