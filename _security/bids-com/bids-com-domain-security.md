---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bids.com
  spf: true
hosts:
- cert_expires: Dec  9 10:24:16 2026 GMT
  host: www.bids.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bids Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bids.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bids.com
provider_slug: bids-com
slug: bids-com-domain-security
source_filename: bids-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bids.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 10:24:16 2026 GMT\n  hsts: false\ndomains:\n- domain: bids.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bids-com/refs/heads/main/security/bids-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Auctions
- Jewelry
- Marketplace
- Retail
---
