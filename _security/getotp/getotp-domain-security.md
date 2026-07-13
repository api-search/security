---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otp.dev
  spf: true
hosts:
- cert_expires: Sep 10 04:08:23 2026 GMT
  host: otp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getotp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetOTP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GetOTP
provider_slug: getotp
slug: getotp-domain-security
source_filename: getotp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:08:23 2026 GMT\n  hsts: false\ndomains:\n- domain: otp.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getotp/refs/heads/main/security/getotp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Authentication And Authorization
- Public APIs
---
