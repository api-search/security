---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alphatrust.com
  spf: true
hosts:
- cert_expires: Dec 30 01:40:02 2026 GMT
  host: alphatrust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alphatrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlphaTrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AlphaTrust
provider_slug: alphatrust
slug: alphatrust-domain-security
source_filename: alphatrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphatrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 01:40:02 2026 GMT\n  hsts: false\ndomains:\n- domain: alphatrust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alphatrust/security/alphatrust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Signature
- Document Automation
- Enterprise
---
