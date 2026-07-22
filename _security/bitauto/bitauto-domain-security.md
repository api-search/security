---
description: ''
domains:
- caa:
  - d2gxho577svb09.cloudfront.net.
  dmarc: false
  dnssec: true
  domain: bitauto.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.bitauto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitauto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitauto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Bitauto
provider_slug: bitauto
slug: bitauto-domain-security
source_filename: bitauto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitauto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bitauto.com\n  dnssec: true\n  caa:\n  - d2gxho577svb09.cloudfront.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitauto/refs/heads/main/security/bitauto-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Consumer
- Automotive
- Cars
- China
- Marketplace
- Digital Marketing
---
