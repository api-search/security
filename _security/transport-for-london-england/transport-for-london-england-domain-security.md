---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tfl.gov.uk
  spf: true
hosts:
- cert_expires: Sep  3 13:45:29 2026 GMT
  host: api.tfl.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For London England Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for London, England, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport for London, England
provider_slug: transport-for-london-england
slug: transport-for-london-england-domain-security
source_filename: transport-for-london-england-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.tfl.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 13:45:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tfl.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-london-england/refs/heads/main/security/transport-for-london-england-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
