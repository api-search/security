---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    agents: []
    checked: '2026-11-27'
    index:
    - alpn:
      - h2
      target: usesideways.com
    published: true
  dnssec: true
  domain: usesideways.com
  spf: false
hosts:
- cert_expires: Jan 13 04:47:49 2027 GMT
  host: usesideways.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sideways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sideways, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Sideways
provider_slug: usesideways-com
slug: usesideways-com-domain-security
source_filename: usesideways-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usesideways.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 04:47:49 2027 GMT\n  hsts: false\ndomains:\n- domain: usesideways.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: true\n    index:\n    - target: usesideways.com\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/usesideways-com/security/usesideways-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI
- Creativity
- LateralThinking
- PromptEngineering
- Tool
---
