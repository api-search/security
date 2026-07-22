---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revion.inc
  spf: true
hosts:
- cert_expires: Oct 17 00:42:47 2026 GMT
  host: revion.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revion
provider_slug: revion
slug: revion-domain-security
source_filename: revion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revion.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: revion.inc\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revion/refs/heads/main/security/revion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Automotive
- Dealership Service
- Voice AI
- Repair Orders
- Workflow Automation
- Y Combinator
---
