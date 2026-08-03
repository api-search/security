---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clicktherapeutics.com
  spf: true
hosts:
- cert_expires: Oct  3 07:49:54 2026 GMT
  host: www.clicktherapeutics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Click Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Click Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Click Therapeutics
provider_slug: click-therapeutics
slug: click-therapeutics-domain-security
source_filename: click-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clicktherapeutics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 07:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clicktherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/click-therapeutics/refs/heads/main/security/click-therapeutics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Therapeutics
- Prescription Digital Therapeutics
- Medical Devices
- Mental Health
- Life Sciences
- Software as a Medical Device
---
