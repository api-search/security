---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: railway.app
  spf: true
hosts:
- cert_expires: Dec 26 03:01:42 2026 GMT
  host: contract-guard-production.up.railway.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contract Guard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contract Guard / Autonomous Utility Factory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contract Guard / Autonomous Utility Factory
provider_slug: contract-guard
slug: contract-guard-domain-security
source_filename: contract-guard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contract-guard-production.up.railway.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:01:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: railway.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contract-guard/refs/heads/main/security/contract-guard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- JSON Validation
- AI Trust
---
