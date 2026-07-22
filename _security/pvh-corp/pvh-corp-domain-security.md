---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:globalnetworkservices@pvh.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pvh.com
  spf: true
hosts:
- cert_expires: Aug 19 00:19:34 2026 GMT
  host: www.pvh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pvh Corp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PVH Corp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PVH Corp
provider_slug: pvh-corp
slug: pvh-corp-domain-security
source_filename: pvh-corp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pvh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pvh.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:globalnetworkservices@pvh.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pvh-corp/refs/heads/main/security/pvh-corp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Brand Portfolio
- Fashion
- Lifestyle
- Public Company
- Retail
- Wholesale
- Fortune 500
---
