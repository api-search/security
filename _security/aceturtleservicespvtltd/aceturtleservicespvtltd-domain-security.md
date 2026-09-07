---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aceturtle.com
  spf: true
hosts:
- cert_expires: Nov  5 09:24:03 2026 GMT
  host: aceturtle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aceturtleservicespvtltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ace Turtle Services Pvt Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ace Turtle Services Pvt Ltd
provider_slug: aceturtleservicespvtltd
slug: aceturtleservicespvtltd-domain-security
source_filename: aceturtleservicespvtltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aceturtle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:24:03 2026 GMT\n  hsts: false\ndomains:\n- domain: aceturtle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aceturtleservicespvtltd/refs/heads/main/security/aceturtleservicespvtltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- E-Commerce
- Omnichannel
- Order Management
- Inventory Management
- Logistics
- Fashion
- India
- SaaS
---
