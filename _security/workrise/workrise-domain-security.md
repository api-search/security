---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rigup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workrise.com
  spf: true
hosts:
- cert_expires: Sep 24 12:45:38 2026 GMT
  host: www.rigup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:29:06 2026 GMT
  host: www.workrise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workrise, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workrise
provider_slug: workrise
slug: workrise-domain-security
source_filename: workrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rigup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:45:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.workrise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:29:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rigup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workrise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workrise/refs/heads/main/security/workrise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Oil And Gas
- Workforce Management
- Vendor Management
- Procurement
- Source To Pay
---
