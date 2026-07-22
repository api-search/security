---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: conocophillips.com
  spf: true
hosts:
- cert_expires: Aug 27 12:34:37 2026 GMT
  host: www.conocophillips.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marathon Oil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marathon Oil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marathon Oil
provider_slug: marathon-oil
slug: marathon-oil-domain-security
source_filename: marathon-oil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conocophillips.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:34:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conocophillips.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marathon-oil/refs/heads/main/security/marathon-oil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Exploration
- Natural Gas
- Oil
- Production
- Fortune 500
---
