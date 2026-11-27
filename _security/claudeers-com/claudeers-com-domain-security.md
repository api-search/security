---
api_specs:
- filename: claudeers-com-openapi-generated.yml
  format: yaml
  label: Claudeers API
  slug: claudeers-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claudeers-com/openapi/_ae-authored/claudeers-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: claudeers.com
  spf: true
hosts:
- cert_expires: Jan 21 21:25:39 2027 GMT
  host: claudeers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claudeers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claudeers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Claudeers
provider_slug: claudeers-com
slug: claudeers-com-domain-security
source_filename: claudeers-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claudeers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 21:25:39 2027 GMT\n  hsts: false\ndomains:\n- domain: claudeers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/claudeers-com/security/claudeers-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Registry
- Community
- Project
- Claude
---
