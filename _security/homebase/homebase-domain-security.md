---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:security@joinhomebase.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinhomebase.com
  spf: true
hosts:
- cert_expires: Sep 28 04:48:47 2026 GMT
  host: www.joinhomebase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: app.joinhomebase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homebase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Homebase
provider_slug: homebase
slug: homebase-domain-security
source_filename: homebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinhomebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:48:47 2026 GMT\n  hsts: false\n- host: app.joinhomebase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinhomebase.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:security@joinhomebase.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homebase/refs/heads/main/security/homebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- scheduling
- time-tracking
- payroll
- HR
- workforce-management
- team-communication
- employee-scheduling
- small-business
- hourly-workers
- integrations
---
