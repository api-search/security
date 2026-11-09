---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: askagent.dev
  spf: true
hosts:
- cert_expires: Dec  5 03:46:34 2026 GMT
  host: askagent.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Askagent Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AskAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AskAgent
provider_slug: askagent-dev
slug: askagent-dev-domain-security
source_filename: askagent-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askagent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 03:46:34 2026 GMT\n  hsts: false\ndomains:\n- domain: askagent.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/askagent-dev/security/askagent-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Platform
- Documentation
- Pricing
- Community
---
