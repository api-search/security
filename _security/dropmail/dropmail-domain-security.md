---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dropmail.me
  spf: true
hosts:
- cert_expires: Oct  8 23:10:37 2026 GMT
  host: dropmail.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropmail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DropMail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DropMail
provider_slug: dropmail
slug: dropmail-domain-security
source_filename: dropmail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dropmail.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:10:37 2026 GMT\n  hsts: false\ndomains:\n- domain: dropmail.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropmail/refs/heads/main/security/dropmail-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Public APIs
---
