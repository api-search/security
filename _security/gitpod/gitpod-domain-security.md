---
api_specs:
- filename: gitpod-environments-openapi.yml
  format: yaml
  label: Gitpod Environments API
  slug: environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitpod/refs/heads/main/openapi/gitpod-environments-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitpod.io
  spf: true
hosts:
- cert_expires: Sep 26 02:12:54 2026 GMT
  host: www.gitpod.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 10:27:02 2026 GMT
  host: api.gitpod.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gitpod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitpod, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gitpod
provider_slug: gitpod
slug: gitpod-domain-security
source_filename: gitpod-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gitpod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:12:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gitpod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 10:27:02 2026 GMT\n  hsts: false\ndomains:\n- domain: gitpod.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitpod/refs/heads/main/security/gitpod-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Cloud Development Environments
- Workspaces
- AI Agents
- DevOps
---
