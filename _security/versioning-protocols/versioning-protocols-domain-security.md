---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: semver.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: calver.org
  spf: false
hosts:
- cert_expires: Sep 17 03:59:51 2026 GMT
  host: semver.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:09:20 2026 GMT
  host: calver.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 16 05:10:07 2026 GMT
  host: www.askantech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Versioning Protocols Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Versioning Protocols, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Versioning Protocols
provider_slug: versioning-protocols
slug: versioning-protocols-domain-security
source_filename: versioning-protocols-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: semver.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:59:51 2026 GMT\n  hsts: false\n- host: calver.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 08:09:20 2026 GMT\n  hsts: false\n- host: www.askantech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 05:10:07 2026 GMT\n  hsts: false\ndomains:\n- domain: semver.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: calver.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versioning-protocols/refs/heads/main/security/versioning-protocols-domain-security.yml
summary_line: TLSv1.3
tags:
- API Design
- Backward Compatibility
- Software Development
- Version Control
- Semantic Versioning
- API Lifecycle
- Deprecation
---
