---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reforge.com
  spf: true
hosts:
- cert_expires: Sep 16 12:01:46 2026 GMT
  host: www.reforge.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:17:48 2026 GMT
  host: docs.reforge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:32:54 2026 GMT
  host: primary.reforge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reforge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reforge
provider_slug: reforge
slug: reforge-domain-security
source_filename: reforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:01:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.reforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:17:48 2026 GMT\n  hsts: false\n- host: primary.reforge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:32:54 2026 GMT\n  hsts: false\ndomains:\n- domain: reforge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reforge/refs/heads/main/security/reforge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Feature Flags
- Feature Management
- Dynamic Configuration
- Live Config
- Experimentation
- Developer Tools
- SDK
- Observability
---
