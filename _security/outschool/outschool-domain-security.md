---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outschool.com
  spf: true
hosts:
- cert_expires: Oct 12 03:24:50 2026 GMT
  host: outschool.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outschool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outschool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outschool
provider_slug: outschool
slug: outschool-domain-security
source_filename: outschool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outschool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:24:50 2026 GMT\n  hsts: false\ndomains:\n- domain: outschool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outschool/refs/heads/main/security/outschool-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Edtech
- Online Learning
- Education
- Marketplace
- Kids
- K-12
- Homeschool
---
