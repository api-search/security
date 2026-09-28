---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: biodesignlab.net
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: biodesignlab.net
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biodesignlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biodesignlab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Biodesignlab
provider_slug: biodesignlab
slug: biodesignlab-domain-security
source_filename: biodesignlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biodesignlab.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: biodesignlab.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biodesignlab/refs/heads/main/security/biodesignlab-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Biotechnology
- Bioengineering
- GeneTherapy
- SyntheticBiology
---
