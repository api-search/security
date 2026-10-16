---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:itsak@sverigesradio.se"
  - 0 issue "telia.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sverigesradio.se
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: sverigesradio.se
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sveriges Radio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sveriges Radio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sveriges Radio
provider_slug: sveriges-radio
slug: sveriges-radio-domain-security
source_filename: sveriges-radio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sverigesradio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: sverigesradio.se\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:itsak@sverigesradio.se\"\n  - 0 issue \"telia.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sveriges-radio/refs/heads/main/security/sveriges-radio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Broadcasting
- Sweden
- Public
---
