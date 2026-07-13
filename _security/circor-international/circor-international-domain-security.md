---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circor.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.circor.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.circor.com
  https: false
- host: api.circor.com
  https: false
kind: domain-security
layout: security
method: probed
name: Circor International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIRCOR International, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CIRCOR International
provider_slug: circor-international
slug: circor-international-domain-security
source_filename: circor-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.circor.com\n  https: false\n- host: api.circor.com\n  https: false\ndomains:\n- domain: circor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circor-international/refs/heads/main/security/circor-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Flow Control
- Industrial
- Energy
---
