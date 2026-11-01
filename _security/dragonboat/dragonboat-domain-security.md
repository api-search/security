---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dragonboat.io
  spf: true
hosts:
- cert_expires: Nov 28 23:23:54 2026 GMT
  host: dragonboat.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dragonboat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dragonboat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dragonboat
provider_slug: dragonboat
slug: dragonboat-domain-security
source_filename: dragonboat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dragonboat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:23:54 2026 GMT\n  hsts: false\ndomains:\n- domain: dragonboat.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dragonboat/security/dragonboat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product Management
- Portfolio Management
- AI Integration
- Enterprise Software
- Agile
---
