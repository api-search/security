---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 1more.com
  spf: true
hosts:
- cert_expires: Oct 26 02:57:32 2026 GMT
  host: usa.1more.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 02:20:11 2027 GMT
  host: www.1more.com
  hsts: false
  hsts_max_age: null
  https: true
  note: 1MORE's corporate site (nginx origin). Probed manually 2026-09-05; not covered by the automated pass because apis.yml carries it as CorporateWebsite. No Strict-Transport-Security header is returned.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 1More Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1MORE, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 1MORE
provider_slug: 1more
slug: 1more-domain-security
source_filename: 1more-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usa.1more.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 02:57:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: www.1more.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 02:20:11 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: 1MORE's corporate site (nginx origin). Probed manually 2026-09-05; not covered by the automated\n    pass because apis.yml carries it as CorporateWebsite. No Strict-Transport-Security header is returned.\ndomains:\n- domain: 1more.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnote: usa.1more.com is the Shopify-hosted US storefront and carries HSTS; www.1more.com is 1MORE's own\n  corporate origin and does not. The apex https://1more.com returned HTTP 504 on every request and global.1more.com\n  did not resolve to a reachable origin, so neither\
  \ could be probed. The registrable domain 1more.com\n  publishes SPF and DMARC but DMARC policy is p=none (monitor only), and there is no DNSSEC and no CAA\n  record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1more/refs/heads/main/security/1more-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
