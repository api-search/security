---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glife.com.sg
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: glifeware.com
  spf: false
hosts:
- cert_expires: Aug 18 07:12:11 2026 GMT
  host: glife.com.sg
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:16:41 2026 GMT
  host: api-sg.glifeware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glife Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glife, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glife
provider_slug: glife
slug: glife-domain-security
source_filename: glife-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glife.com.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:12:11 2026 GMT\n  hsts: false\n- host: api-sg.glifeware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:16:41 2026 GMT\n  hsts: false\ndomains:\n- domain: glife.com.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: glifeware.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glife/refs/heads/main/security/glife-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Tech
- Grocery
- Supply Chain
- E-Commerce
- GraphQL
- Southeast Asia
- AgTech
- Logistics
---
