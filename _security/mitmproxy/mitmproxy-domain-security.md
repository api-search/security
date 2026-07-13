---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mitmproxy.org
  spf: true
hosts:
- cert_expires: Sep 26 16:12:46 2026 GMT
  host: mitmproxy.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:12:46 2026 GMT
  host: docs.mitmproxy.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mitmproxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mitmproxy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mitmproxy
provider_slug: mitmproxy
slug: mitmproxy-domain-security
source_filename: mitmproxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mitmproxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:12:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.mitmproxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:12:46 2026 GMT\n  hsts: null\ndomains:\n- domain: mitmproxy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitmproxy/refs/heads/main/security/mitmproxy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Testing
- HTTP Debugging
- HTTPS Proxy
- Open Source
- Security Testing
- Traffic Analysis
- Traffic Interception
---
