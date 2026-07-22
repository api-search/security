---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polarsignals.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buf.build
  spf: true
hosts:
- cert_expires: Sep 30 15:57:53 2026 GMT
  host: www.polarsignals.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 00:46:30 2026 GMT
  host: buf.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:43:10 2026 GMT
  host: api.polarsignals.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polar Signals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polar Signals, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Polar Signals
provider_slug: polar-signals
slug: polar-signals-domain-security
source_filename: polar-signals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polarsignals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:57:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: buf.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:46:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.polarsignals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:43:10 2026 GMT\n  hsts: null\ndomains:\n- domain: polarsignals.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: buf.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar-signals/refs/heads/main/security/polar-signals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Observability
- Continuous Profiling
- Performance
- eBPF
- gRPC
- Developer Tools
- MCP
- GPU
---
