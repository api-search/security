---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bastille.net
  spf: true
hosts:
- cert_expires: Sep 23 09:47:09 2026 GMT
  host: www.bastille.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bastille Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bastille Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bastille Networks
provider_slug: bastille-networks
slug: bastille-networks-domain-security
source_filename: bastille-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bastille.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bastille.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bastille-networks/refs/heads/main/security/bastille-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Wireless Security
- RF Detection
- Wireless Airspace
- IoT Security
- OT Security
- Threat Detection
---
