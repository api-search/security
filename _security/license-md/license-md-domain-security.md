---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: choosealicense.com
  spf: true
hosts:
- cert_expires: Oct  1 14:02:51 2026 GMT
  host: choosealicense.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: License Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LICENSE.md, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LICENSE.md
provider_slug: license-md
slug: license-md-domain-security
source_filename: license-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: choosealicense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: choosealicense.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/license-md/refs/heads/main/security/license-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Legal
- Licensing
- Open Source
- SPDX
- License
---
