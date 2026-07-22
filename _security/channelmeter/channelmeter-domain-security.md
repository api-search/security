---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: channelmeter.com
  spf: true
hosts:
- cert_expires: Sep 25 06:10:20 2026 GMT
  host: channelmeter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channelmeter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChannelMeter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChannelMeter
provider_slug: channelmeter
slug: channelmeter-domain-security
source_filename: channelmeter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channelmeter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:10:20 2026 GMT\n  hsts: false\ndomains:\n- domain: channelmeter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelmeter/refs/heads/main/security/channelmeter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Creator Economy
- Creator Management
- Payments
- Payouts
- Analytics
- Influencer Marketing
- Fintech
---
