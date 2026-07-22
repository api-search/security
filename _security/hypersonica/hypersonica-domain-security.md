---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hypersonica.com
  spf: true
hosts:
- cert_expires: Jan  8 19:52:28 2027 GMT
  host: hypersonica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hypersonica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypersonica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hypersonica
provider_slug: hypersonica
slug: hypersonica-domain-security
source_filename: hypersonica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypersonica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 19:52:28 2027 GMT\n  hsts: null\ndomains:\n- domain: hypersonica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hypersonica/refs/heads/main/security/hypersonica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defense
- Aerospace
- Hypersonics
- Defence Technology
- Deep Tech
- Munich
---
