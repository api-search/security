---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: g2.com
  spf: true
hosts:
- cert_expires: Sep 23 20:58:38 2026 GMT
  host: documentation.g2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 06:00:00 2026 GMT
  host: data.g2.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: G2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G2, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: G2
provider_slug: g2
slug: g2-domain-security
source_filename: g2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: documentation.g2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.g2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: g2.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2/refs/heads/main/security/g2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Software Discovery
- Software Reviews
---
