---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: varnish-cache.org
  spf: false
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: varnish-cache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Varnish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Varnish Cache, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Varnish Cache
provider_slug: varnish
slug: varnish-domain-security
source_filename: varnish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: varnish-cache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: varnish-cache.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varnish/refs/heads/main/security/varnish-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Caching
- Caching Proxy
- Content Delivery
- HTTP Accelerator
- Open Source
- Proxy
- Reverse Proxy
---
