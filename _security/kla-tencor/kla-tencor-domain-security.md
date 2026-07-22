---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kla.com
  spf: true
hosts:
- cert_expires: Sep 17 02:00:46 2026 GMT
  host: www.kla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kla Tencor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KLA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KLA
provider_slug: kla-tencor
slug: kla-tencor-domain-security
source_filename: kla-tencor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:00:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kla.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kla-tencor/refs/heads/main/security/kla-tencor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Semiconductors
- Manufacturing
- Metrology
- Inspection
- Process Control
---
