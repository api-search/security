---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vastrm.com
  spf: true
hosts:
- cert_expires: Sep 26 05:08:41 2026 GMT
  host: vastrm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vastrm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vastrm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vastrm
provider_slug: vastrm
slug: vastrm-domain-security
source_filename: vastrm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vastrm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 05:08:41 2026 GMT\n  hsts: false\ndomains:\n- domain: vastrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vastrm/refs/heads/main/security/vastrm-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Apparel
- Fashion
- eCommerce
- Retail
- Custom Clothing
- Menswear
---
