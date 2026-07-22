---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: planetfwd.com
  spf: true
hosts:
- cert_expires: Sep 10 09:37:50 2026 GMT
  host: www.planetfwd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planet Fwd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planet FWD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Planet FWD
provider_slug: planet-fwd
slug: planet-fwd-domain-security
source_filename: planet-fwd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planetfwd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:37:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: planetfwd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planet-fwd/refs/heads/main/security/planet-fwd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate
- Sustainability
- Carbon Accounting
- Decarbonization
- Life Cycle Assessment
- CPG
- Supply Chain
---
