---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pulsecharterconnect.com
  spf: true
hosts:
- cert_expires: Aug 28 05:42:54 2026 GMT
  host: pulsecharterconnect.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Charter Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse Charter Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pulse Charter Connect
provider_slug: pulse-charter-connect
slug: pulse-charter-connect-domain-security
source_filename: pulse-charter-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulsecharterconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:42:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: pulsecharterconnect.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-charter-connect/refs/heads/main/security/pulse-charter-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
