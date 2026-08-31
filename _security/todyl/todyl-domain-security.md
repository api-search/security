---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: todyl.com
  spf: true
hosts:
- cert_expires: Oct 13 20:13:19 2026 GMT
  host: www.todyl.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 14:08:06 2026 GMT
  host: api.todyl.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Todyl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Todyl, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Todyl
provider_slug: todyl
slug: todyl-domain-security
source_filename: todyl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.todyl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.todyl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 14:08:06 2026 GMT\n  hsts: null\ndomains:\n- domain: todyl.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todyl/refs/heads/main/security/todyl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security
- Managed Service Providers
- SASE
- SIEM
- Endpoint Security
- Managed Detection and Response
- Governance Risk and Compliance
- Zero Trust
- Networking
---
