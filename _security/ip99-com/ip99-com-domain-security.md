---
description: ''
domains:
- caa:
  - ip99.com.cdn.dnsv1.com.
  - 6bdvze36.slt.sched.intlscdn.com.
  dmarc: false
  dnssec: true
  domain: ip99.com
  spf: false
hosts:
- cert_expires: Dec  8 20:59:59 2026 GMT
  host: ip99.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IP99 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP99, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: IP99
provider_slug: ip99-com
slug: ip99-com-domain-security
source_filename: ip99-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ip99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 20:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ip99.com\n  dnssec: true\n  caa:\n  - ip99.com.cdn.dnsv1.com.\n  - 6bdvze36.slt.sched.intlscdn.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ip99-com/security/ip99-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- IP risk
- Geolocation
- Phone-number risk
- Passive DNS
- Certificate Transparency
- Self-Hosted
---
