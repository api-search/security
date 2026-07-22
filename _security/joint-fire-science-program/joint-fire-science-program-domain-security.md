---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: firescience.gov
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.firescience.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joint Fire Science Program Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joint Fire Science Program, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Joint Fire Science Program
provider_slug: joint-fire-science-program
slug: joint-fire-science-program-domain-security
source_filename: joint-fire-science-program-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firescience.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: firescience.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joint-fire-science-program/refs/heads/main/security/joint-fire-science-program-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Fire Science
- Fires
- Wildfire
- Research
---
