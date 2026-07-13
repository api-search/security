---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heico.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.heico.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.heico.com
  https: false
- host: api.heico.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HEICO Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HEICO Corporation
provider_slug: heico
slug: heico-domain-security
source_filename: heico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\n- host: developer.heico.com\n  https: false\n- host: api.heico.com\n  https: false\ndomains:\n- domain: heico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heico/refs/heads/main/security/heico-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Aviation
- Defense
---
