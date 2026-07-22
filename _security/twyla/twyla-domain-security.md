---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: twyla.com
  spf: true
hosts:
- cert_expires: Sep 18 16:04:26 2026 GMT
  host: twyla.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twyla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twyla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Twyla
provider_slug: twyla
slug: twyla-domain-security
source_filename: twyla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twyla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:04:26 2026 GMT\n  hsts: false\ndomains:\n- domain: twyla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twyla/refs/heads/main/security/twyla-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Art
- Marketplace
- Art Prints
- E-Commerce
---
