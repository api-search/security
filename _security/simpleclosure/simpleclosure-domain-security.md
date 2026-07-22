---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simpleclosure.com
  spf: true
hosts:
- cert_expires: Sep 13 01:15:11 2026 GMT
  host: simpleclosure.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simpleclosure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simpleclosure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Simpleclosure
provider_slug: simpleclosure
slug: simpleclosure-domain-security
source_filename: simpleclosure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpleclosure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:15:11 2026 GMT\n  hsts: false\ndomains:\n- domain: simpleclosure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpleclosure/refs/heads/main/security/simpleclosure-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Business Dissolution
- Startup Shutdown
- Wind Down
- Legal Tech
- Fintech
- Compliance
---
