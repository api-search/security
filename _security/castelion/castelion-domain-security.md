---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: castelion.com
  spf: true
hosts:
- cert_expires: Aug 21 12:45:03 2026 GMT
  host: www.castelion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Castelion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castelion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Castelion
provider_slug: castelion
slug: castelion-domain-security
source_filename: castelion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.castelion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:45:03 2026 GMT\n  hsts: false\ndomains:\n- domain: castelion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castelion/refs/heads/main/security/castelion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defense
- Aerospace
- Hypersonics
- Manufacturing
- Weapons Systems
- National Security
---
