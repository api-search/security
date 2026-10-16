---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codeldoors.com
  spf: true
hosts:
- cert_expires: Dec  2 02:11:59 2026 GMT
  host: www.codeldoors.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codel Doors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codel Doors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Codel Doors
provider_slug: codel-doors
slug: codel-doors-domain-security
source_filename: codel-doors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codeldoors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 02:11:59 2026 GMT\n  hsts: false\ndomains:\n- domain: codeldoors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codel-doors/refs/heads/main/security/codel-doors-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Doors
- Fiberglass Doors
- Steel Doors
- Patio Doors
- Interior Doors
- Door Distribution
---
