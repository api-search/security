---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: metromile.com
  spf: true
hosts:
- cert_expires: Sep  4 08:46:50 2026 GMT
  host: www.metromile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: enterprise.metromile.com
  https: false
kind: domain-security
layout: security
method: probed
name: Metromile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metromile, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Metromile
provider_slug: metromile
slug: metromile-domain-security
source_filename: metromile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metromile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 08:46:50 2026 GMT\n  hsts: null\n- host: enterprise.metromile.com\n  https: false\ndomains:\n- domain: metromile.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metromile/refs/heads/main/security/metromile-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Telematics
- Pay-Per-Mile
- Auto Insurance
- Claims Automation
- Vehicle Diagnostics
- Mileage Tracking
- InsurTech
---
