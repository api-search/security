---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chemours.com
  spf: true
hosts:
- cert_expires: Apr 25 23:59:59 2027 GMT
  host: www.chemours.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chemours Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chemours, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chemours
provider_slug: chemours
slug: chemours-domain-security
source_filename: chemours-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chemours.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: chemours.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chemours/refs/heads/main/security/chemours-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chemicals
- Manufacturing
- Fluoropolymers
- Refrigerants
- Titanium Dioxide
- Fortune 1000
---
