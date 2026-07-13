---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: netscout.com
  spf: true
hosts:
- cert_expires: Jul 20 23:59:59 2026 GMT
  host: my.netscout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.netscout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netscout, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Netscout
provider_slug: netscout
slug: netscout-domain-security
source_filename: netscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: my.netscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.netscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netscout.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netscout/refs/heads/main/security/netscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- DDoS Protection
- Network Monitoring
- Network Performance
- Service Assurance
- Threat Intelligence
---
