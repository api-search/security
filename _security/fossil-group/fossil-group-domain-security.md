---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fossilgroup.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fossil.com
  spf: true
hosts:
- cert_expires: Aug 25 11:29:48 2026 GMT
  host: www.fossilgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 02:46:26 2026 GMT
  host: www.fossil.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 13 02:01:49 2026 GMT
  host: www.skagen.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fossil Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fossil Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fossil Group
provider_slug: fossil-group
slug: fossil-group-domain-security
source_filename: fossil-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fossilgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:29:48 2026 GMT\n  hsts: null\n- host: www.fossil.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 02:46:26 2026 GMT\n  hsts: null\n- host: www.skagen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 02:01:49 2026 GMT\n  hsts: null\ndomains:\n- domain: fossilgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fossil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossil-group/refs/heads/main/security/fossil-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fashion
- Accessories
- Watches
- Wearables
- Retail
- Fortune 1000
---
