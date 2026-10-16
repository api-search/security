---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lansforsakringar.se
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: lansforsakringar.se
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lansforsakringar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Länsförsäkringar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Länsförsäkringar
provider_slug: lansforsakringar
slug: lansforsakringar-domain-security
source_filename: lansforsakringar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lansforsakringar.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: lansforsakringar.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lansforsakringar/refs/heads/main/security/lansforsakringar-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Insurance
- Financial Services
- Sweden
---
