---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: trucks.vc
  spf: true
hosts:
- cert_expires: Sep  9 15:48:19 2026 GMT
  host: trucks.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trucks Venture Fund I Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trucks Venture Fund I, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Trucks Venture Fund I
provider_slug: trucks-venture-fund-i
slug: trucks-venture-fund-i-domain-security
source_filename: trucks-venture-fund-i-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trucks.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 15:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trucks.vc\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trucks-venture-fund-i/refs/heads/main/security/trucks-venture-fund-i-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Venture Capital
- Investment
- Transportation
- Mobility
- Autonomous Vehicles
- Early Stage
---
