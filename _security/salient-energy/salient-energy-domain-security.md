---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salientenergyinc.com
  spf: true
hosts:
- cert_expires: Oct 17 09:35:45 2026 GMT
  host: salientenergyinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salient Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salient Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Salient Energy
provider_slug: salient-energy
slug: salient-energy-domain-security
source_filename: salient-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salientenergyinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:35:45 2026 GMT\n  hsts: false\ndomains:\n- domain: salientenergyinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salient-energy/refs/heads/main/security/salient-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Energy Storage
- Battery
- Zinc-Ion Battery
- Clean Energy
- Climate Tech
- Manufacturing
- Hardware
---
