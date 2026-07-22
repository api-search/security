---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: masterclass.com
  spf: true
hosts:
- cert_expires: Oct  7 17:54:59 2026 GMT
  host: www.masterclass.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Masterclass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MasterClass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MasterClass
provider_slug: masterclass
slug: masterclass-domain-security
source_filename: masterclass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.masterclass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:54:59 2026 GMT\n  hsts: null\ndomains:\n- domain: masterclass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/masterclass/refs/heads/main/security/masterclass-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Education
- Online Learning
- Streaming
- Video
- E-Learning
- Professional Development
---
