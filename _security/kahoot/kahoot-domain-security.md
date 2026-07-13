---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kahoot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kahoot.it
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: kahoot.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:42:23 2026 GMT
  host: support.kahoot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: apis.kahoot.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kahoot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kahoot!, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kahoot!
provider_slug: kahoot
slug: kahoot-domain-security
source_filename: kahoot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kahoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: support.kahoot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:42:23 2026 GMT\n  hsts: null\n- host: apis.kahoot.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kahoot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kahoot.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kahoot/refs/heads/main/security/kahoot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Game-Based Learning
- Education
- Quiz
- Engagement
- Enterprise Learning
- Reporting
- OAuth
---
