---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marlinequity.com
  spf: true
hosts:
- cert_expires: Aug 31 19:23:53 2026 GMT
  host: marlinequity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marlinequity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marlin Equity Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marlin Equity Partners
provider_slug: marlinequity
slug: marlinequity-domain-security
source_filename: marlinequity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marlinequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:23:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marlinequity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marlinequity/refs/heads/main/security/marlinequity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Private Equity
- Investment
- Technology
- Software
- Financial Technology
- Mergers and Acquisitions
---
