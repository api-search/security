---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cal.com
  spf: true
hosts:
- cert_expires: Sep 14 15:26:52 2026 GMT
  host: cal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:46:41 2026 GMT
  host: api.cal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cal.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cal.com
provider_slug: calcom
slug: calcom-domain-security
source_filename: calcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cal.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calcom/refs/heads/main/security/calcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Scheduling
- Calendars
- Bookings
- Open Source
- Event Types
---
