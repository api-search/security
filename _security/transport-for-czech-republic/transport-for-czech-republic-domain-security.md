---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: chaps.cz
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.chaps.cz
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Czech Republic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Czech Republic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Transport for Czech Republic
provider_slug: transport-for-czech-republic
slug: transport-for-czech-republic-domain-security
source_filename: transport-for-czech-republic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chaps.cz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chaps.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-czech-republic/refs/heads/main/security/transport-for-czech-republic-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
