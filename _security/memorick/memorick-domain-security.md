---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: memorick.com
  spf: false
hosts:
- cert_expires: Oct 17 15:48:41 2026 GMT
  host: memorick.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memorick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memorick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Memorick
provider_slug: memorick
slug: memorick-domain-security
source_filename: memorick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memorick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 15:48:41 2026 GMT\n  hsts: false\ndomains:\n- domain: memorick.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memorick/refs/heads/main/security/memorick-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Photography
- Booking
- Marketplace
- Travel
- Photographers
- OAuth
- Laravel
---
