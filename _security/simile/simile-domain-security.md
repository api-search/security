---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simile.ai
  spf: false
hosts:
- cert_expires: Sep 20 01:40:04 2026 GMT
  host: simile.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Simile
provider_slug: simile
slug: simile-domain-security
source_filename: simile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simile.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:40:04 2026 GMT\n  hsts: false\ndomains:\n- domain: simile.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simile/refs/heads/main/security/simile-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Apps
- Simulation
- Human Behavior
- Consumer Insights
- Market Research
- Foundation Model
- Behavioral Science
- Synthetic Users
- Artificial Intelligence
---
