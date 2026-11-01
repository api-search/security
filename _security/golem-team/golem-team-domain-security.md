---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: golem.team
  spf: true
hosts:
- cert_expires: Dec 19 01:03:35 2026 GMT
  host: golem.team
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Golem Team Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for golem-team, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: golem-team
provider_slug: golem-team
slug: golem-team-domain-security
source_filename: golem-team-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golem.team\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:03:35 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: golem.team\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/golem-team/security/golem-team-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Security
- Agent
- Detection
- Response
---
