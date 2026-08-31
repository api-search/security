---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: group1auto.com
  spf: true
hosts:
- cert_expires: Oct  5 18:45:34 2026 GMT
  host: www.group1auto.com
  hsts: true
  hsts_max_age: 3000
  hsts_note: 'Strict-Transport-Security: max-age=3000 observed on https://www.group1auto.com/llms.txt (200) on 2026-08-28. The automated probe recorded null because Cloudflare bot management answers 403 to the site root for non-browser clients; the header is present on paths that are served. max-age=3000 (50 minutes) is far below the 31536000 recommended for preload eligibility.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Group 1 Automotive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Group 1 Automotive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Group 1 Automotive
provider_slug: group-1-automotive
slug: group-1-automotive-domain-security
source_filename: group-1-automotive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.group1auto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:45:34 2026 GMT\n  hsts: true\n  hsts_max_age: 3000\n  hsts_note: 'Strict-Transport-Security: max-age=3000 observed on https://www.group1auto.com/llms.txt\n    (200) on 2026-08-28. The automated probe recorded null because Cloudflare bot management answers 403\n    to the site root for non-browser clients; the header is present on paths that are served. max-age=3000\n    (50 minutes) is far below the 31536000 recommended for preload eligibility.'\ndomains:\n- domain: group1auto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes: group-1-automotive.com does not resolve (NXDOMAIN) and was the Website pointer in apis.yml before\n  this pass; the live corporate/retail host is www.group1auto.com, served by the Cars.com / Dealer Inspire\n  platform\
  \ behind Cloudflare. Investor site www.group1corp.com is a Notified investorroom.com tenant.\n  UK operations run on www.group1auto.co.uk (Azure Front Door). No CAA record and no DNSSEC on group1auto.com;\n  DMARC is published at p=none (monitor only, no enforcement).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/group-1-automotive/refs/heads/main/security/group-1-automotive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Automotive
- Automotive Retail
- Vehicle Inventory
- Dealerships
- Retail
- Agentic Access
- llms-txt
---
