---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nist.gov
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spiffe.io
  spf: false
hosts:
- cert_expires: Sep 24 09:16:11 2026 GMT
  host: www.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 05:17:40 2026 GMT
  host: spiffe.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 19:18:56 2026 GMT
  host: www.openpolicyagent.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zero Trust Architecture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zero Trust Architecture, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zero Trust Architecture
provider_slug: zero-trust-architecture
slug: zero-trust-architecture-domain-security
source_filename: zero-trust-architecture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:16:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spiffe.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 05:17:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.openpolicyagent.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:18:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nist.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spiffe.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-trust-architecture/refs/heads/main/security/zero-trust-architecture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Control
- Authentication
- Authorization
- Cybersecurity
- Identity Management
- Least Privilege
- Network Security
- NIST
- Security
- Zero Trust
---
