---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@faultkey.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: faultkey.com
  spf: true
hosts:
- cert_expires: Dec 10 19:15:41 2026 GMT
  host: faultkey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faultkey Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FaultKey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FaultKey
provider_slug: faultkey-com
slug: faultkey-com-domain-security
source_filename: faultkey-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faultkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 19:15:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: faultkey.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@faultkey.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/faultkey-com/security/faultkey-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Liability
- Governance
- Bitcoin
- MCP
---
