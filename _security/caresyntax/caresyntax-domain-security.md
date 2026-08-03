---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caresyntax.com
  spf: true
hosts:
- cert_expires: Oct  7 00:02:30 2026 GMT
  host: www.caresyntax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.caresyntax.com
  hsts: null
  https: true
  note: Kong 3.4.2 API gateway (CNAME api.new.caresyntax.com); every probed path returns HTTP 404 {"message":"no Route matched with those values"} — no public route, no spec, no /.well-known/ documents.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caresyntax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caresyntax, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caresyntax
provider_slug: caresyntax
slug: caresyntax-domain-security
source_filename: caresyntax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caresyntax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:02:30 2026 GMT\n  hsts: null\n- host: api.caresyntax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\n  note: 'Kong 3.4.2 API gateway (CNAME api.new.caresyntax.com); every probed path\n    returns HTTP 404 {\"message\":\"no Route matched with those values\"} — no public\n    route, no spec, no /.well-known/ documents.'\ndomains:\n- domain: caresyntax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caresyntax/refs/heads/main/security/caresyntax-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Surgery
- Surgical Intelligence
- Operating Room
- Medical Devices
- MedTech
- Analytics
- Artificial Intelligence
- Health Data
- Interoperability
---
