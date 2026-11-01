---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: raindrop.io
  spf: true
hosts:
- cert_expires: Dec 16 13:10:06 2026 GMT
  host: raindrop.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raindrop Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raindrop.io (bookmarks), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Raindrop.io (bookmarks)
provider_slug: raindrop-io
slug: raindrop-io-domain-security
source_filename: raindrop-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raindrop.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 13:10:06 2026 GMT\n  hsts: false\ndomains:\n- domain: raindrop.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/raindrop-io/security/raindrop-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bookmark
- Productivity
- Cloud
- Collaboration
- API
---
