---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: point.com
  spf: true
hosts:
- cert_expires: Oct 14 21:22:15 2026 GMT
  host: point.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Point Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Point, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Point
provider_slug: point
slug: point-domain-security
source_filename: point-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: point.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:22:15 2026 GMT\n  hsts: false\ndomains:\n- domain: point.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/point/refs/heads/main/security/point-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Home Equity
- Mortgage
- Lending
- Real Estate
- Consumer Finance
- HELOC
---
