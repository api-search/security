---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: constanellis.com
  spf: true
hosts:
- cert_expires: Dec 25 04:14:28 2026 GMT
  host: www.constanellis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constanellisaerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constanellisaerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Constanellisaerospace
provider_slug: constanellisaerospace
slug: constanellisaerospace-domain-security
source_filename: constanellisaerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.constanellis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 04:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: constanellis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constanellisaerospace/refs/heads/main/security/constanellisaerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Space
- Infrastructure
- Cislunar
- Manufacturing
---
