---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kodemsecurity.com
  spf: true
hosts:
- cert_expires: Oct 14 00:19:16 2026 GMT
  host: www.kodemsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 13:31:50 2026 GMT
  host: docs.kodemsecurity.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 09:16:09 2026 GMT
  host: api.kodemsecurity.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  note: HSTS observed on the authenticated 401 response (strict-transport-security max-age=15724800; includeSubDomains); the unauthenticated HEAD probe did not surface the header.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kodem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kodem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kodem
provider_slug: kodem
slug: kodem-domain-security
source_filename: kodem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kodemsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 00:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kodemsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 13:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.kodemsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 09:16:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  note: HSTS observed on the authenticated 401 response (strict-transport-security max-age=15724800;\n    includeSubDomains); the unauthenticated HEAD probe did not surface the header.\ndomains:\n- domain: kodemsecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kodem/refs/heads/main/security/kodem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Application Security
- Runtime Security
- Software Composition Analysis
- Static Analysis
- Vulnerability Management
- DevSecOps
- SBOM
- AI Security
---
