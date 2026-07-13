---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: togatech.org
  spf: true
hosts:
- cert_expires: Oct  4 21:07:53 2026 GMT
  host: uselection.togatech.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Presidential Election Data By Togatech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Presidential Election Data by TogaTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: US Presidential Election Data by TogaTech
provider_slug: us-presidential-election-data-by-togatech
slug: us-presidential-election-data-by-togatech-domain-security
source_filename: us-presidential-election-data-by-togatech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uselection.togatech.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:07:53 2026 GMT\n  hsts: false\ndomains:\n- domain: togatech.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-presidential-election-data-by-togatech/refs/heads/main/security/us-presidential-election-data-by-togatech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
