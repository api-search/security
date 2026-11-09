---
api_specs:
- filename: clearly-sh-openapi-generated.yml
  format: yaml
  label: Clearly API
  slug: clearly-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearly-sh/openapi/_ae-authored/clearly-sh-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clearly.sh
  spf: true
hosts:
- cert_expires: Dec 10 04:29:48 2026 GMT
  host: clearly.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clearly Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Clearly
provider_slug: clearly-sh
slug: clearly-sh-domain-security
source_filename: clearly-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearly.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clearly.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clearly-sh/security/clearly-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Workspace
- Design Tools
---
