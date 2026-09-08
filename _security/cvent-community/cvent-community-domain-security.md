---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "comodo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cvent.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 03:08:29 2026 GMT
  host: community.cvent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: support.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: release.cvent.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: status.cvent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Cvent Community Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cvent Community, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cvent Community
provider_slug: cvent-community
slug: cvent-community-domain-security
source_filename: cvent-community-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; community.cvent.com, support.cvent.com, release.cvent.com\n  and status.cvent.com probed by the enrichment pass 2026-09-07\nhosts:\n- host: www.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: community.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 03:08:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: release.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: status.cvent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain:\
  \ cvent.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-community/refs/heads/main/security/cvent-community-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Certification
- Community
- Customer-Support
- Cvent Academy
- Education
- Forums
- Knowledge Base
- Learning Centers
- Software-as-a-Service
- Training
---
