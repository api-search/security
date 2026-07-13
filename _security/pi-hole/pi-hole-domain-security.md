---
api_specs:
- filename: docs
  format: yaml
  label: Pi-hole REST API
  slug: rest-api
  spec_type: OpenAPI
  url: http://pi.hole/api/docs
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:servers@pi-hole.net"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pi-hole.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pi.hole
  spf: false
hosts:
- cert_expires: Oct  6 04:50:35 2026 GMT
  host: pi-hole.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:53:46 2026 GMT
  host: docs.pi-hole.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: pi.hole
  https: false
kind: domain-security
layout: security
method: probed
name: Pi Hole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pi-hole, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pi-hole
provider_slug: pi-hole
slug: pi-hole-domain-security
source_filename: pi-hole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pi-hole.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:50:35 2026 GMT\n  hsts: false\n- host: docs.pi-hole.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:53:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pi.hole\n  https: false\ndomains:\n- domain: pi-hole.net\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:servers@pi-hole.net\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pi.hole\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pi-hole/refs/heads/main/security/pi-hole-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- Ad Blocking
- Network Security
- Privacy
- Open Source
- Self-Hosted
---
