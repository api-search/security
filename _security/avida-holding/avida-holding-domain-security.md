---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avida.ae
  spf: true
hosts:
- cert_expires: Dec  2 20:03:44 2026 GMT
  host: avida.ae
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avida Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avida Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avida Holding
provider_slug: avida-holding
slug: avida-holding-domain-security
source_filename: avida-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avida.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 20:03:44 2026 GMT\n  hsts: false\ndomains:\n- domain: avida.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avida-holding/refs/heads/main/security/avida-holding-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Lending
- Sweden
- Norway
- Finland
---
