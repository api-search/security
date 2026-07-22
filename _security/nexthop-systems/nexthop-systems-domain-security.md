---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexthop.ai
  spf: true
hosts:
- cert_expires: Aug 28 03:13:35 2026 GMT
  host: nexthop.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nexthop Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexthop Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexthop Systems
provider_slug: nexthop-systems
slug: nexthop-systems-domain-security
source_filename: nexthop-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexthop.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 03:13:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexthop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthop-systems/refs/heads/main/security/nexthop-systems-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Networking
- AI Infrastructure
- Data Center
- Ethernet Switches
- Optics and Cables
- Networking Hardware
- Hyperscaler
---
