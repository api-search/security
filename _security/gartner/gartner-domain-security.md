---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gartner.com
  spf: true
hosts:
- cert_expires: Aug 14 05:00:45 2026 GMT
  host: www.gartner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gartner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gartner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gartner
provider_slug: gartner
slug: gartner-domain-security
source_filename: gartner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gartner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 05:00:45 2026 GMT\n  hsts: false\ndomains:\n- domain: gartner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gartner/refs/heads/main/security/gartner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Research
- Advisory
- Analyst
- Enterprise
- Fortune 1000
---
