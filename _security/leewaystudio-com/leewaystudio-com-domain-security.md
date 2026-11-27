---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leewaystudio.com
  spf: true
hosts:
- cert_expires: Dec 17 15:46:59 2026 GMT
  host: leewaystudio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leeway Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leeway Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Leeway Studio
provider_slug: leewaystudio-com
slug: leewaystudio-com-domain-security
source_filename: leewaystudio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leewaystudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:46:59 2026 GMT\n  hsts: false\ndomains:\n- domain: leewaystudio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leewaystudio-com/security/leewaystudio-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Productivity
- CognitiveLoad
- Tools
- Experiments
- Community
---
