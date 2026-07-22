---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: speedlancer.com
  spf: true
hosts:
- cert_expires: Sep  6 14:28:40 2026 GMT
  host: speedlancer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speedlancer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speedlancer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Speedlancer
provider_slug: speedlancer
slug: speedlancer-domain-security
source_filename: speedlancer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speedlancer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:28:40 2026 GMT\n  hsts: false\ndomains:\n- domain: speedlancer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speedlancer/refs/heads/main/security/speedlancer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Freelance
- Marketplace
- Gig Economy
- 500 Global
---
