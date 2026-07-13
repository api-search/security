---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cfindustries.com
  spf: true
hosts:
- cert_expires: Sep 14 02:55:00 2026 GMT
  host: www.cfindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cf Industries Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CF Industries Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CF Industries Holdings
provider_slug: cf-industries-holdings
slug: cf-industries-holdings-domain-security
source_filename: cf-industries-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cfindustries.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 02:55:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cfindustries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cf-industries-holdings/refs/heads/main/security/cf-industries-holdings-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Agriculture
- Ammonia
- Chemicals
- Clean Energy
- Fertilizer
- Fortune 500
- Hydrogen
- Investor Relations
- Low-Carbon
- Manufacturing
- Nitrogen
- Supply Chain
---
