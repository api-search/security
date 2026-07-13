---
api_specs:
- filename: windsurf-enterprise-openapi.yml
  format: yaml
  label: Windsurf Enterprise API
  slug: windsurf-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windsurfrules/refs/heads/main/openapi/windsurf-enterprise-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: windsurf.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codeium.com
  spf: true
hosts:
- cert_expires: Sep  6 12:51:55 2026 GMT
  host: windsurf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:31:21 2026 GMT
  host: docs.windsurf.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:42:07 2026 GMT
  host: server.codeium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Windsurfrules Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windsurf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Windsurf
provider_slug: windsurfrules
slug: windsurfrules-domain-security
source_filename: windsurfrules-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: windsurf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 12:51:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.windsurf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:31:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: server.codeium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:42:07 2026 GMT\n  hsts: null\ndomains:\n- domain: windsurf.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: codeium.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windsurfrules/refs/heads/main/security/windsurfrules-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- AI Copilot
- Coding Standards
- Developer Workflow
- IDE
- Windsurf
---
