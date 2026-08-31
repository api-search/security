---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sprpainrelief.com
  spf: true
hosts:
- cert_expires: Oct  5 23:12:58 2026 GMT
  host: www.sprpainrelief.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spr Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPR Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SPR Therapeutics
provider_slug: spr-therapeutics
slug: spr-therapeutics-domain-security
source_filename: spr-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sprpainrelief.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:12:58 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: sprpainrelief.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spr-therapeutics/refs/heads/main/security/spr-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Neuromodulation
- Pain Management
- Neurotechnology
- Medical Technology
---
