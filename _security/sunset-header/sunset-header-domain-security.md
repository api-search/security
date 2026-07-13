---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rfc-editor.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 05:02:36 2026 GMT
  host: www.rfc-editor.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunset Header Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunset Header, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sunset Header
provider_slug: sunset-header
slug: sunset-header-domain-security
source_filename: sunset-header-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: www.rfc-editor.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:02:36 2026 GMT\n  hsts: false\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rfc-editor.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunset-header/refs/heads/main/security/sunset-header-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Deprecation
- HTTP Headers
- RFC 8594
- RFC 9745
- API Lifecycle
- REST APIs
- Standards
---
