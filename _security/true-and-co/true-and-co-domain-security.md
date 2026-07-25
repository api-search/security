---
description: ''
domains: []
hosts: []
kind: domain-security
layout: security
method: probed
name: True And Co Domain Security
name_suffix: Domain Security
overview: Domain security posture for True & Co, probed live across 0 host(s) and 0 registrable domain(s).
provider_name: True & Co
provider_slug: true-and-co
slug: true-and-co-domain-security
source_filename: true-and-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: 2026-07-21\nmethod: probed\nsource: live TLS handshake, HTTP response headers, and DNS lookups on 2026-07-21\ndomain: trueandco.com\ntls:\n  present: true\n  issuer: \"Let's Encrypt (CN=YE2)\"\n  not_before: '2026-06-09'\n  not_after: '2026-09-07'\nhsts:\n  present: true\n  header: max-age=7889238\n  max_age: 7889238\n  include_subdomains: false\n  preload: false\ncsp:\n  present: true\n  header: \"block-all-mixed-content; frame-ancestors 'none'; upgrade-insecure-requests;\"\nspf:\n  present: true\n  record: \"v=spf1 include:spf-00778a01.pphosted.com include:mail.zendesk.com ~all\"\ndmarc:\n  present: true\n  policy: none\n  record: \"v=DMARC1; p=none; rua=mailto:dmarc_agg@pvh.com; ruf=mailto:dmarc_afrf@pvh.com; fo=1\"\ncaa:\n  present: true\n  records:\n  - '0 issue \"digicert.com\"'\n  - '0 issue \"globalsign.com\"'\n  - '0 issue \"godaddy.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 iodef \"globalnetworkservices@pvh.com\"'\ndnssec:\n  present: false\n  note:\
  \ No DS record published at the parent zone.\nmx:\n  present: true\n  records:\n  - mxb-00778a01.gslb.pphosted.com (Proofpoint)\n  - mxa-00778a01.gslb.pphosted.com (Proofpoint)\nnotes: >-\n  Storefront served via Cloudflare on Shopify infrastructure. DMARC aggregation and\n  CAA iodef contacts resolve to pvh.com, consistent with True & Co operating under\n  PVH Corp. Corporate mail is routed through Proofpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-and-co/refs/heads/main/security/true-and-co-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Apparel
- Intimates
- Agentic Commerce
- Shopify
- MCP
---
