---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appliedvr.io
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: appliedvr.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appliedvr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppliedVR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppliedVR
provider_slug: appliedvr
slug: appliedvr-domain-security
source_filename: appliedvr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appliedvr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: appliedvr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appliedvr/refs/heads/main/security/appliedvr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Therapeutics
- Virtual Reality
- Healthcare
- Medical Device
- Chronic Pain
- Behavioral Health
---
