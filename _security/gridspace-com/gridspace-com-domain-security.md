---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gridspace.com
  spf: true
hosts:
- cert_expires: Dec  7 17:32:11 2026 GMT
  host: www.gridspace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gridspace Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gridspace
provider_slug: gridspace-com
slug: gridspace-com-domain-security
source_filename: gridspace-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gridspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:32:11 2026 GMT\n  hsts: false\ndomains:\n- domain: gridspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gridspace-com/security/gridspace-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Voice AI
- API
- Regulated Compliance
- Healthcare
- Insurance
- Fintech
- Government
- BPO
---
