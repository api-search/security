---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: builddirect.com
  spf: true
hosts:
- cert_expires: Nov 10 05:43:32 2026 GMT
  host: www.builddirect.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Builddirect Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildDirect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BuildDirect
provider_slug: builddirect-technologies
slug: builddirect-technologies-domain-security
source_filename: builddirect-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.builddirect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 05:43:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: builddirect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builddirect-technologies/refs/heads/main/security/builddirect-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Flooring
- Home Improvement
- Building Materials
- Trade Services
---
