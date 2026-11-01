---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oemsecrets.com
  spf: true
hosts:
- cert_expires: Dec 21 21:44:54 2026 GMT
  host: www.oemsecrets.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oemsecrets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OEMsecrets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OEMsecrets
provider_slug: oemsecrets
slug: oemsecrets-domain-security
source_filename: oemsecrets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oemsecrets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 21:44:54 2026 GMT\n  hsts: null\ndomains:\n- domain: oemsecrets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oemsecrets/security/oemsecrets-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
