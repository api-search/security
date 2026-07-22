---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sandhillmarkets.com
  spf: true
hosts:
- cert_expires: Aug 28 00:31:27 2026 GMT
  host: sandhillmarkets.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stonks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stonks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Stonks
provider_slug: stonks
slug: stonks-domain-security
source_filename: stonks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sandhillmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:31:27 2026 GMT\n  hsts: null\ndomains:\n- domain: sandhillmarkets.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stonks/refs/heads/main/security/stonks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Private Markets
- Secondaries
- Investing
- Fintech
- Venture Capital
- Pre-IPO
---
