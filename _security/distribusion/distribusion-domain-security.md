---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:infrastructure@distribusion.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: distribusion.com
  spf: true
hosts:
- cert_expires: Sep 21 04:50:53 2026 GMT
  host: distribusion.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Distribusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distribusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Distribusion
provider_slug: distribusion
slug: distribusion-domain-security
source_filename: distribusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distribusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:50:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: distribusion.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:infrastructure@distribusion.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distribusion/refs/heads/main/security/distribusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transportation
- Travel
- Mobility
- Ground Travel
- Booking
- Distribution
- API
---
