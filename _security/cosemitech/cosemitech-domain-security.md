---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cosemitech.com
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: www.cosemitech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosemitech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosemitech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cosemitech
provider_slug: cosemitech
slug: cosemitech-domain-security
source_filename: cosemitech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cosemitech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cosemitech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosemitech/refs/heads/main/security/cosemitech-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Semiconductor
- IC
- Automotive
- Industrial
- Energy
- Consumer Electronics
- Company
---
