---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: snapsheet.com
  spf: true
hosts:
- cert_expires: Nov 14 02:42:43 2026 GMT
  host: snapsheet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bodyshopbids Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bodyshopbids, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bodyshopbids
provider_slug: bodyshopbids
slug: bodyshopbids-domain-security
source_filename: bodyshopbids-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 02:42:43 2026 GMT\n  hsts: false\ndomains:\n- domain: snapsheet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bodyshopbids/refs/heads/main/security/bodyshopbids-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Automotive
- Claims
- B2B
- Platform
---
