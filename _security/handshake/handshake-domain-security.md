---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joinhandshake.com
  spf: true
hosts:
- cert_expires: Sep 19 07:31:47 2026 GMT
  host: www.joinhandshake.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Handshake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handshake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Handshake
provider_slug: handshake
slug: handshake-domain-security
source_filename: handshake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinhandshake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:31:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinhandshake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handshake/refs/heads/main/security/handshake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- Careers
- Recruiting
- Higher Education
- Talent
- Students
- Jobs
---
