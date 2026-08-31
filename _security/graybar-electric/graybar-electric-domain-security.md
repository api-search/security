---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: graybar.com
  spf: true
hosts:
- cert_expires: Oct 31 20:41:07 2026 GMT
  host: www.graybar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 20:41:07 2026 GMT
  host: apiportal-snd.graybar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Graybar Electric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graybar Electric, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Graybar Electric
provider_slug: graybar-electric
slug: graybar-electric-domain-security
source_filename: graybar-electric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graybar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 20:41:07 2026 GMT\n  hsts: null\n- host: apiportal-snd.graybar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 20:41:07 2026 GMT\n  hsts: null\ndomains:\n- domain: graybar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graybar-electric/refs/heads/main/security/graybar-electric-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Fortune 500
- Distribution
- Electrical
- Data Networking
- Supply Chain
- Logistics
- B2B eCommerce
- EDI
- PunchOut
- Industrial
---
