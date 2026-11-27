---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bilgai.com
  spf: true
hosts:
- cert_expires: Jan 25 22:36:57 2027 GMT
  host: bilgai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bilg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bilg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bilg
provider_slug: bilgai-com
slug: bilgai-com-domain-security
source_filename: bilgai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bilgai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 22:36:57 2027 GMT\n  hsts: false\ndomains:\n- domain: bilgai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bilgai-com/security/bilgai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Collaboration
- Knowledge Base
- Productivity
- Team Workspace
---
