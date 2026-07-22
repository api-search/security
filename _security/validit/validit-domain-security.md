---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: validit.ai
  spf: false
  txt_notes:
  - amazonses domain verification present
  - postman-domain-verification TXT present (no public Postman workspace found)
hosts:
- cert_expires: Sep 28 08:50:17 2026 GMT
  host: validit.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.validit.ai
  hsts: false
  https: true
  note: Live production API host (NestJS-style JSON 404 envelope); no public spec or docs.
  tls_version: TLSv1.3
- cert_expires: Nov 9 23:59:59 2026 GMT
  host: app.validit.ai
  hsts: false
  https: true
  note: Web-based assessment app (React SPA on CloudFront).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Validit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valid.it, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Valid.it
provider_slug: validit
slug: validit-domain-security
source_filename: validit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: validit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:50:17 2026 GMT\n  hsts: false\n- host: api.validit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n  note: Live production API host (NestJS-style JSON 404 envelope); no public spec or docs.\n- host: app.validit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 9 23:59:59 2026 GMT\n  hsts: false\n  note: Web-based assessment app (React SPA on CloudFront).\ndomains:\n- domain: validit.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  txt_notes:\n  - amazonses domain verification present\n  - postman-domain-verification TXT present (no public Postman workspace found)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validit/refs/heads/main/security/validit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fraud Prevention
- Identity Verification
- Deepfake Detection
- Deception Detection
- Artificial Intelligence
- KYC
- Security
---
