---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonicwall.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: www.sonicwall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonicwall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SonicWall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SonicWall
provider_slug: sonicwall
slug: sonicwall-domain-security
source_filename: sonicwall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonicwall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sonicwall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonicwall/refs/heads/main/security/sonicwall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Network Security
- Firewall
- Next-Generation Firewall
- Intrusion Prevention
- VPN
- SD-WAN
- SASE
- Cloud Secure Edge
- Zero Trust
- Endpoint Security
- Email Security
- Cloud Email Security
- Managed Detection and Response
- MSSP
- Sandbox
- Capture ATP
- SonicOS
- SMB
---
