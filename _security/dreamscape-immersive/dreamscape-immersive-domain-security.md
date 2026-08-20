---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dreamscapeimmersive.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: techscapevr.com
  spf: false
hosts:
- cert_expires: Oct  6 22:31:52 2026 GMT
  host: dreamscapeimmersive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.techscapevr.com
  hsts: false
  http_status: 403
  https: true
  note: production AWS API Gateway backend; anonymous requests refused
  tls_version: TLSv1.3
- host: api.hq.dev.techscapevr.com
  hsts: false
  http_status: 403
  https: true
  note: development AWS API Gateway backend named by REACT_APP_API_DOMAIN in the shipped bundle
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dreamscape Immersive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dreamscape Immersive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dreamscape Immersive
provider_slug: dreamscape-immersive
slug: dreamscape-immersive-domain-security
source_filename: dreamscape-immersive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the backend hosts named in the\n  dreamscapeimmersive.com JavaScript bundle\nnote: >-\n  techscapevr.com is Dreamscape Immersive's engineering domain — the consumer site's React\n  bundle (static/js/main.a6db2b7f.chunk.js) resolves REACT_APP_API_DOMAIN to hosts under it.\n  Both API hosts are AWS API Gateway endpoints that answer 403 {\"message\":\"Forbidden\"} to\n  every anonymous request, so only transport-layer posture could be probed. The apex\n  techscapevr.com does not resolve over HTTPS at all (DNS failure) — only the api.* and\n  assets.* subdomains exist. No SPF TXT record is published at the techscapevr.com apex,\n  DMARC is present but at p=none (monitor only), and there is no CAA record or DNSSEC on\n  either domain.\nhosts:\n- host: dreamscapeimmersive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:31:52 2026 GMT\n  hsts: false\n- host: api.techscapevr.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n  http_status: 403\n  note: production AWS API Gateway backend; anonymous requests refused\n- host: api.hq.dev.techscapevr.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  http_status: 403\n  note: development AWS API Gateway backend named by REACT_APP_API_DOMAIN in the shipped bundle\ndomains:\n- domain: dreamscapeimmersive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: techscapevr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dreamscape-immersive/refs/heads/main/security/dreamscape-immersive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Virtual Reality
- Immersive Experiences
- Location-Based Entertainment
- Entertainment
- Media
- Ticketing
- Education Technology
---
