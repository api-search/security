---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fractera.ai
  spf: false
hosts:
- cert_expires: Dec 28 21:28:38 2026 GMT
  host: fractera.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fractera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fractera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Fractera
provider_slug: fractera-ai
slug: fractera-ai-domain-security
source_filename: fractera-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fractera.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 21:28:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fractera.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fractera-ai/security/fractera-ai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Platform
- Self-Hosted
- Open Source
---
