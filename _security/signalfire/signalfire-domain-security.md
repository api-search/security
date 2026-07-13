---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signalfire.com
  spf: true
hosts:
- cert_expires: Aug 19 00:11:18 2026 GMT
  host: signalfire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signalfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignalFire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SignalFire
provider_slug: signalfire
slug: signalfire-domain-security
source_filename: signalfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signalfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:11:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signalfire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signalfire/refs/heads/main/security/signalfire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Venture Capital
- Investment
- Startup Funding
- Private Markets
- Beacon AI
- Talent Intelligence
- Go To Market Intelligence
- Sourcing
---
