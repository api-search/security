---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: authshore.ai
  spf: true
hosts:
- cert_expires: Jan  3 22:37:40 2027 GMT
  host: authshore.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Authshore Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AuthShore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AuthShore
provider_slug: authshore-ai
slug: authshore-ai-domain-security
source_filename: authshore-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authshore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 22:37:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: authshore.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/authshore-ai/security/authshore-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Artificial Intelligence
- Developer Tools
- Security
---
