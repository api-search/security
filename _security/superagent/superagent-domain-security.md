---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superagent.sh
  spf: true
hosts:
- cert_expires: Oct  5 20:14:55 2026 GMT
  host: www.superagent.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuperAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SuperAgent
provider_slug: superagent
slug: superagent-domain-security
source_filename: superagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superagent.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:14:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: superagent.sh\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superagent/refs/heads/main/security/superagent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Automation
---
