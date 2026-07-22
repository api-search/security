---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: caremerge.com
  spf: true
hosts:
- cert_expires: Sep 30 11:28:47 2026 GMT
  host: www.caremerge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caremerge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareMerge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CareMerge
provider_slug: caremerge
slug: caremerge-domain-security
source_filename: caremerge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caremerge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:28:47 2026 GMT\n  hsts: false\ndomains:\n- domain: caremerge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caremerge/refs/heads/main/security/caremerge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Senior Living
- Care Coordination
- Family Engagement
- Long-Term Care
- Community Engagement
- Health Technology
---
