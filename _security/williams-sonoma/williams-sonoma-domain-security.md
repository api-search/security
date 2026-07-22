---
description: ''
domains:
- caa:
  - 128 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: williams-sonoma.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: www.williams-sonoma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Williams Sonoma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Williams-Sonoma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Williams-Sonoma
provider_slug: williams-sonoma
slug: williams-sonoma-domain-security
source_filename: williams-sonoma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.williams-sonoma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: williams-sonoma.com\n  dnssec: false\n  caa:\n  - 128 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/williams-sonoma/refs/heads/main/security/williams-sonoma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- E-Commerce
- Home Furnishings
- Kitchenware
- Fortune 500
---
