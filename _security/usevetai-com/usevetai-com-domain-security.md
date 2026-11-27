---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usevetai.com
  spf: true
hosts:
- cert_expires: Dec 28 16:24:31 2026 GMT
  host: usevetai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: VetAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VetAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VetAI
provider_slug: usevetai-com
slug: usevetai-com-domain-security
source_filename: usevetai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usevetai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 16:24:31 2026 GMT\n  hsts: null\ndomains:\n- domain: usevetai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usevetai-com/security/usevetai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Automation
- Finance
- Support
- Operations
---
