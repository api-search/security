---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: utilidata.com
  spf: true
hosts:
- cert_expires: Oct 10 08:03:16 2026 GMT
  host: utilidata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Jul  7 09:08:39 2026 GMT
  cert_issuer: C=US, O=Let's Encrypt, CN=R12
  cert_not_before: Apr  8 09:08:40 2026 GMT
  cert_subject: CN=developer.utilidata.com
  host: developer.utilidata.com
  hsts: null
  https: false
  tls_version: TLSv1.3
  x-finding: EXPIRED CERTIFICATE. The Karman developer host has been serving an expired Let's Encrypt certificate since 2026-07-07 — every browser, crawler and agent gets a TLS error rather than the site. Probed manually on 2026-08-05 (curl exit 60); the host is not listed in apis.yml because it is unreachable, so the automated probe does not cover it.
kind: domain-security
layout: security
method: probed
name: Utilidata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utilidata, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Utilidata
provider_slug: utilidata
slug: utilidata-domain-security
source_filename: utilidata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilidata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:03:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.utilidata.com\n  https: false\n  tls_version: TLSv1.3\n  cert_subject: CN=developer.utilidata.com\n  cert_issuer: 'C=US, O=Let''s Encrypt, CN=R12'\n  cert_not_before: Apr  8 09:08:40 2026 GMT\n  cert_expires: Jul  7 09:08:39 2026 GMT\n  cert_expired: true\n  hsts: null\n  x-finding: >-\n    EXPIRED CERTIFICATE. The Karman developer host has been serving an expired Let's\n    Encrypt certificate since 2026-07-07 — every browser, crawler and agent gets a TLS\n    error rather than the site. Probed manually on 2026-08-05 (curl exit 60); the host is\n    not listed in apis.yml because it is unreachable, so the automated probe does not\n    cover it.\ndomains:\n- domain: utilidata.com\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilidata/refs/heads/main/security/utilidata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electric Grid
- Utilities
- Data Centers
- Artificial Intelligence
- Edge Computing
- Telemetry
- Protocol Buffers
- Open-Source
- Grid Edge
- Power Quality
---
