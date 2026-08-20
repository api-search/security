---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bendingspoons.com
  spf: true
hosts:
- cert_expires: Oct 11 14:00:54 2026 GMT
  host: bendingspoons.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bending Spoons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bending Spoons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bending Spoons
provider_slug: bending-spoons
slug: bending-spoons-domain-security
source_filename: bending-spoons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bendingspoons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:00:54 2026 GMT\n  hsts: false\ndomains:\n- domain: bendingspoons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bending-spoons/refs/heads/main/security/bending-spoons-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Holding Company
- Consumer Apps
- Mobile Apps
- Software
- Software-as-a-Service
- Acquisitions
- Publicly Traded
- Italy
- Portfolio
---
