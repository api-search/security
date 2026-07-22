---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stagwellglobal.com
  spf: true
hosts:
- cert_expires: Aug 25 16:19:38 2026 GMT
  host: www.stagwellglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stagwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stagwell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stagwell
provider_slug: stagwell
slug: stagwell-domain-security
source_filename: stagwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stagwellglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:19:38 2026 GMT\n  hsts: false\ndomains:\n- domain: stagwellglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stagwell/refs/heads/main/security/stagwell-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing
- Advertising
- Media
- MarTech
---
