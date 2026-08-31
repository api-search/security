---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gowalla.com
  spf: true
hosts:
- cert_expires: Sep 13 00:26:39 2026 GMT
  host: gowalla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gowalla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gowalla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Gowalla
provider_slug: gowalla
slug: gowalla-domain-security
source_filename: gowalla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gowalla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:26:39 2026 GMT\n  hsts: null\ndomains:\n- domain: gowalla.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gowalla/refs/heads/main/security/gowalla-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Consumer
- Location
- Social
- Check-In
- Mobile
- Geolocation
- Maps
---
