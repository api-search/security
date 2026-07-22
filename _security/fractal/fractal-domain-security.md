---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fractalsoftware.com
  spf: true
hosts:
- cert_expires: Sep 25 10:48:01 2026 GMT
  host: fractalsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fractal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fractal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fractal
provider_slug: fractal
slug: fractal-domain-security
source_filename: fractal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fractalsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:48:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fractalsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fractal/refs/heads/main/security/fractal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Venture Studio
- Vertical SaaS
- Artificial Intelligence
- Startups
- Incubator
- Enterprise Software
---
