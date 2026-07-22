---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lenskart.com
  spf: true
hosts:
- cert_expires: Oct  7 03:47:23 2026 GMT
  host: www.lenskart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:47:23 2026 GMT
  host: api.lenskart.com
  hsts: false
  https: true
  note: host resolves and terminates TLS but returns HTTP 404 at the root; no public API is documented behind it
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:20:11 2026 GMT
  host: blog.lenskart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lenskart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lenskart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lenskart
provider_slug: lenskart
slug: lenskart-domain-security
source_filename: lenskart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lenskart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:47:23 2026 GMT\n  hsts: false\n- host: api.lenskart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:47:23 2026 GMT\n  hsts: false\n  note: host resolves and terminates TLS but returns HTTP 404 at the root; no public\n    API is documented behind it\n- host: blog.lenskart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:20:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lenskart.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lenskart/refs/heads/main/security/lenskart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Retail
- E-Commerce
- Eyewear
- Direct to Consumer
- Optical
- Omnichannel
---
