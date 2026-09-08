---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: advance-composite.co.jp
  spf: true
hosts:
- cert_expires: Oct 23 10:10:21 2026 GMT
  host: advance-composite.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advancecomposite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advance Composite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Advance Composite
provider_slug: advancecomposite
slug: advancecomposite-domain-security
source_filename: advancecomposite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advance-composite.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 10:10:21 2026 GMT\n  hsts: false\ndomains:\n- domain: advance-composite.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancecomposite/refs/heads/main/security/advancecomposite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Materials Science
- Advanced Materials
- Metal Matrix Composites
- Thermal Management
- Semiconductors
- Aluminum
- Japan
---
