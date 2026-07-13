---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ivanti.com
  spf: true
hosts:
- cert_expires: Oct  5 00:49:15 2026 GMT
  host: www.ivanti.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:49:15 2026 GMT
  host: help.ivanti.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pulse
provider_slug: pulse
slug: pulse-domain-security
source_filename: pulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ivanti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.ivanti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ivanti.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse/refs/heads/main/security/pulse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Ivanti
- Network Security
- Secure Access
- SSL VPN
- VPN
- Zero Trust
---
