---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marathonpetroleum.com
  spf: true
hosts:
- cert_expires: Aug 22 10:40:00 2026 GMT
  host: www.marathonpetroleum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marathon Petroleum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marathon Petroleum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marathon Petroleum
provider_slug: marathon-petroleum
slug: marathon-petroleum-domain-security
source_filename: marathon-petroleum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marathonpetroleum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:40:00 2026 GMT\n  hsts: null\ndomains:\n- domain: marathonpetroleum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marathon-petroleum/refs/heads/main/security/marathon-petroleum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Fortune 500
- Petroleum
- Pipelines
- Refining
---
