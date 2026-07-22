---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cambridgeaerospace.com
  spf: true
hosts:
- cert_expires: Oct 14 05:48:13 2026 GMT
  host: www.cambridgeaerospace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cambridge Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cambridge Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cambridge Aerospace
provider_slug: cambridge-aerospace
slug: cambridge-aerospace-domain-security
source_filename: cambridge-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cambridgeaerospace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:48:13 2026 GMT\n  hsts: false\ndomains:\n- domain: cambridgeaerospace.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cambridge-aerospace/refs/heads/main/security/cambridge-aerospace-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- Defense
- Aerospace
- Missile Defense
- Interceptors
- Hardware
- United Kingdom
---
