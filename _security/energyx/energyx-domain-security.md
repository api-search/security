---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energyx.com
  spf: true
hosts:
- cert_expires: Sep 28 12:24:36 2026 GMT
  host: energyx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Energyx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnergyX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EnergyX
provider_slug: energyx
slug: energyx-domain-security
source_filename: energyx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: energyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:24:36 2026 GMT\n  hsts: false\ndomains:\n- domain: energyx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/security/energyx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lithium
- Direct Lithium Extraction
- Critical Minerals
- Battery Technology
- Energy Transition
- Cleantech
- Materials Science
- Mining
- Chemicals
- Nuclear Materials
- Manufacturing
---
