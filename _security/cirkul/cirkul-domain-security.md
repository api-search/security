---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drinkcirkul.com
  spf: true
hosts:
- cert_expires: Oct 24 00:55:32 2026 GMT
  host: drinkcirkul.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cirkul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cirkul, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cirkul
provider_slug: cirkul
slug: cirkul-domain-security
source_filename: cirkul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drinkcirkul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 00:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: drinkcirkul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cirkul/refs/heads/main/security/cirkul-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Direct to Consumer
- Ecommerce
- Retail
- Subscription Commerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Hydration
---
