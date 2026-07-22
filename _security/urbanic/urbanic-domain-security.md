---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: urbanic.com
  spf: true
hosts:
- cert_expires: Aug 14 07:29:14 2026 GMT
  host: in.urbanic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urbanic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Urbanic
provider_slug: urbanic
slug: urbanic-domain-security
source_filename: urbanic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: in.urbanic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 07:29:14 2026 GMT\n  hsts: null\ndomains:\n- domain: urbanic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanic/refs/heads/main/security/urbanic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ecommerce
- Fashion
- Apparel
- Retail
- Consumer
---
