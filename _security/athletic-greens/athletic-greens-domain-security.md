---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drinkag1.com
  spf: true
hosts:
- cert_expires: Oct  9 22:44:32 2026 GMT
  host: drinkag1.com
  hsts: null
  https: true
  note: edge answered HTTP 429 to every non-browser request probed on 2026-08-02
  tls_version: TLSv1.3
- cert_expires: Oct 28 06:10:02 2026 GMT
  host: shop.drinkag1.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 18:04:01 2026 GMT
  host: account.drinkag1.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athletic Greens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AG1, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AG1
provider_slug: athletic-greens
slug: athletic-greens-domain-security
source_filename: athletic-greens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nnote: ucp.dev is referenced as the humanURL of the UCP commerce endpoint but is the\n  protocol's own host, not an AG1-controlled domain, so it is excluded here.\nhosts:\n- host: drinkag1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:44:32 2026 GMT\n  hsts: null\n  note: edge answered HTTP 429 to every non-browser request probed on 2026-08-02\n- host: shop.drinkag1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 06:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: account.drinkag1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 18:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: drinkag1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletic-greens/refs/heads/main/security/athletic-greens-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Health
- Nutrition
- Supplements
- Direct to Consumer
- Ecommerce
- Subscription
- Wellness
- Agentic Commerce
- MCP
- UCP
- Shopify
- GraphQL
---
