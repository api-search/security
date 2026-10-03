---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blue.world
  spf: true
hosts:
- cert_expires: Oct 30 09:33:38 2026 GMT
  host: www.blue.world
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blueworldtechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueworldtechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blueworldtechnologies
provider_slug: blueworldtechnologies
slug: blueworldtechnologies-domain-security
source_filename: blueworldtechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blue.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 09:33:38 2026 GMT\n  hsts: false\ndomains:\n- domain: blue.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueworldtechnologies/refs/heads/main/security/blueworldtechnologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Fuel Cells
- Maritime
- Renewables
---
