---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jd.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: jdcloud.com
  spf: false
hosts:
- cert_expires: Dec 20 04:28:34 2026 GMT
  host: open.jd.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 04:28:34 2026 GMT
  host: api.jd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:05:24 2026 GMT
  host: docs.jdcloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jd Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JD.com (Jingdong), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JD.com (Jingdong)
provider_slug: jd-com
slug: jd-com-domain-security
source_filename: jd-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.jd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 04:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: api.jd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 04:28:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.jdcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: jdcloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jd-com/refs/heads/main/security/jd-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-commerce
- Marketplace
- China
- Cloud Platform
- Logistics
- Retail
- JD Open Platform
- JD Cloud
- JOS
---
