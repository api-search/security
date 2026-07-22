---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parseplatform.org
  spf: true
hosts:
- cert_expires: Oct  3 22:40:35 2026 GMT
  host: parseplatform.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:40:35 2026 GMT
  host: docs.parseplatform.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parse
provider_slug: parse
slug: parse-domain-security
source_filename: parse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parseplatform.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:40:35 2026 GMT\n  hsts: false\n- host: docs.parseplatform.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:40:35 2026 GMT\n  hsts: false\ndomains:\n- domain: parseplatform.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parse/refs/heads/main/security/parse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Backend as a Service
- BaaS
- Mobile
- Open Source
- REST API
- Database
- Authentication
- Push Notifications
- Real Time
---
