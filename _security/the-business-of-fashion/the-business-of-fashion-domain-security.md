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
  domain: businessoffashion.com
  spf: true
hosts:
- cert_expires: Oct 15 13:27:21 2026 GMT
  host: businessoffashion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Business Of Fashion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Business of Fashion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Business of Fashion
provider_slug: the-business-of-fashion
slug: the-business-of-fashion-domain-security
source_filename: the-business-of-fashion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: businessoffashion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:27:21 2026 GMT\n  hsts: false\ndomains:\n- domain: businessoffashion.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-business-of-fashion/refs/heads/main/security/the-business-of-fashion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Fashion
- Publishing
- News
- Intelligence
- Luxury
---
