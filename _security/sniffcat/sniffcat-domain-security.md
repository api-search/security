---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sniffcat.com
  spf: true
hosts:
- cert_expires: Oct  5 23:43:17 2026 GMT
  host: sniffcat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:43:17 2026 GMT
  host: api.sniffcat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sniffcat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SniffCat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SniffCat
provider_slug: sniffcat
slug: sniffcat-domain-security
source_filename: sniffcat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sniffcat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:43:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sniffcat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:43:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sniffcat.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sniffcat/refs/heads/main/security/sniffcat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Threat Intelligence
- ip-reputation
- abuse-database
- Cybersecurity
- OSINT
- network-security
- sysadmin-tools
- Blocklist
- abuse-reporting
- ip-blocklist
- ip-intelligence
- threat-feeds
---
