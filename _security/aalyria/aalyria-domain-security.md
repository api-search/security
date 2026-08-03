---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aalyria.com
  spf: true
hosts:
- cert_expires: Sep 11 16:00:21 2026 GMT
  host: www.aalyria.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:57:27 2026 GMT
  host: docs.spacetime.aalyria.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: nbi.example.spacetime.aalyria.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aalyria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aalyria, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aalyria
provider_slug: aalyria
slug: aalyria-domain-security
source_filename: aalyria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aalyria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:00:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spacetime.aalyria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:57:27 2026 GMT\n  hsts: false\n- host: nbi.example.spacetime.aalyria.com\n  https: false\ndomains:\n- domain: aalyria.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aalyria/refs/heads/main/security/aalyria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Networking
- Satellite
- Space
- Telecommunications
- Software Defined Networking
- Orchestration
- Aerospace
- Defense
- Connectivity
- gRPC
- Protocol Buffers
- Telemetry
- Optical Communications
---
