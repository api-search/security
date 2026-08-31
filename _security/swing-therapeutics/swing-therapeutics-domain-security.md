---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swingtherapeutics.com
  spf: true
hosts:
- cert_expires: Nov 20 22:25:53 2026 GMT
  host: swingtherapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swing Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swing Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swing Therapeutics
provider_slug: swing-therapeutics
slug: swing-therapeutics-domain-security
source_filename: swing-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swingtherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 22:25:53 2026 GMT\n  hsts: false\ndomains:\n- domain: swingtherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swing-therapeutics/refs/heads/main/security/swing-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Therapeutics
- Health
- Healthcare
- Digital Health
- Fibromyalgia
- Chronic Pain
- Behavioral Health
- Prescription Digital Therapeutic
- Telemedicine
- Mobile Application
- No Public API
---
