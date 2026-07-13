---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: graylog.org
  spf: true
hosts:
- cert_expires: Aug 27 17:42:21 2026 GMT
  host: graylog.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.graylog.org
  https: false
kind: domain-security
layout: security
method: probed
name: Graylog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graylog, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Graylog
provider_slug: graylog
slug: graylog-domain-security
source_filename: graylog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graylog.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:42:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.graylog.org\n  https: false\ndomains:\n- domain: graylog.org\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graylog/refs/heads/main/security/graylog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logging
- Observability
- Log Management
- SIEM
---
