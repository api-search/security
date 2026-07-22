---
api_specs:
- filename: stakpak-openapi-original.yml
  format: yaml
  label: Stakpak API
  slug: stakpak-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stakpak/refs/heads/main/openapi/stakpak-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stakpak.dev
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: stakpak.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: apiv2.stakpak.dev
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stakpak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StakPak, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: StakPak
provider_slug: stakpak
slug: stakpak-domain-security
source_filename: stakpak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stakpak.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: apiv2.stakpak.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: stakpak.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stakpak/refs/heads/main/security/stakpak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- DevOps
- Infrastructure
- AI Agents
- MCP
- Developer Tools
- CLI
- Cloud
---
