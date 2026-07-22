---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hyster-yale.com
  spf: true
hosts:
- cert_expires: Aug 28 17:33:32 2026 GMT
  host: www.hyster-yale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyster Yale Materials Handling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyster-Yale Materials Handling, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hyster-Yale Materials Handling
provider_slug: hyster-yale-materials-handling
slug: hyster-yale-materials-handling-domain-security
source_filename: hyster-yale-materials-handling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyster-yale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:33:32 2026 GMT\n  hsts: false\ndomains:\n- domain: hyster-yale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyster-yale-materials-handling/refs/heads/main/security/hyster-yale-materials-handling-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Forklifts
- Materials Handling
- Industrial
- Manufacturing
- Logistics
---
