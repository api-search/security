---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinreal.com
  spf: true
hosts:
- cert_expires: Sep 16 00:16:29 2026 GMT
  host: www.joinreal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Real Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Real, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Real
provider_slug: real
slug: real-domain-security
source_filename: real-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinreal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:16:29 2026 GMT\n  hsts: false\ndomains:\n- domain: joinreal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/real/refs/heads/main/security/real-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
