---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umpquabank.com
  spf: true
hosts:
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: www.umpquabank.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: developer.umpquabank.com
  https: false
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: api.umpquabank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umpqua Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umpqua Holdings, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Umpqua Holdings
provider_slug: umpqua-holdings
slug: umpqua-holdings-domain-security
source_filename: umpqua-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.umpquabank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: null\n- host: developer.umpquabank.com\n  https: false\n- host: api.umpquabank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: umpquabank.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umpqua-holdings/refs/heads/main/security/umpqua-holdings-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Banking
- Financial Services
---
