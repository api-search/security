---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bodyfriend.com
  spf: true
hosts:
- cert_expires: Dec  2 03:49:31 2026 GMT
  host: bodyfriend.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bodyfriend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bodyfriend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bodyfriend
provider_slug: bodyfriend
slug: bodyfriend-domain-security
source_filename: bodyfriend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bodyfriend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:49:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bodyfriend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyfriend/refs/heads/main/security/bodyfriend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Massage Chairs
- Home Wellness
- Rehabilitation
- Healthcare Technology
---
