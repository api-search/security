---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: thesiftguide.com
  spf: true
hosts:
- cert_expires: Feb 24 05:38:06 2027 GMT
  host: thesiftguide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Sift Minecraft Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Sift Minecraft Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Sift Minecraft Guide
provider_slug: thesiftguide-com
slug: thesiftguide-com-domain-security
source_filename: thesiftguide-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesiftguide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 05:38:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thesiftguide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/thesiftguide-com/security/thesiftguide-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Minecraft
- Wiki
- Community
- Dimension
- Guide
---
