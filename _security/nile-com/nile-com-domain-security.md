---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nilesecure.com
  spf: true
hosts:
- cert_expires: Aug 19 21:25:05 2026 GMT
  host: nilesecure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: my.nilesecure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nile Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nile
provider_slug: nile-com
slug: nile-com-domain-security
source_filename: nile-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nilesecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:25:05 2026 GMT\n  hsts: false\n- host: my.nilesecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nilesecure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nile-com/refs/heads/main/security/nile-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Networking
- Enterprise Networking
- Network As A Service
- NaaS
- Wi-Fi
- LAN
- Campus Networking
- Branch Networking
- Zero Trust
- Zero Trust Networking
- SASE
- SSE
- Network Security
- Network Automation
- AIOps
- AI Native Networking
- Autonomous Networking
- Cloud Managed Networking
- Digital Twin
- Webhooks
---
