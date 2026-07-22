---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ucp.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: skullcandy.com
  spf: true
hosts:
- cert_expires: Sep  6 11:38:51 2026 GMT
  host: ucp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:51:34 2026 GMT
  host: www.skullcandy.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:37:15 2026 GMT
  host: shopify.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skullcandy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skullcandy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skullcandy
provider_slug: skullcandy
slug: skullcandy-domain-security
source_filename: skullcandy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ucp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:38:51 2026 GMT\n  hsts: false\n- host: www.skullcandy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:51:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ucp.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skullcandy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skullcandy/refs/heads/main/security/skullcandy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- MCP
- Universal Commerce Protocol
---
