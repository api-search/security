---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: topgolfcallawaybrands.com
  spf: true
hosts:
- cert_expires: Aug 19 05:25:53 2026 GMT
  host: www.topgolfcallawaybrands.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Topgolf Callaway Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Topgolf Callaway Brands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Topgolf Callaway Brands
provider_slug: topgolf-callaway-brands
slug: topgolf-callaway-brands-domain-security
source_filename: topgolf-callaway-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.topgolfcallawaybrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:25:53 2026 GMT\n  hsts: null\ndomains:\n- domain: topgolfcallawaybrands.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topgolf-callaway-brands/refs/heads/main/security/topgolf-callaway-brands-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Golf
- Entertainment
- Sports Equipment
- Fortune 500
---
