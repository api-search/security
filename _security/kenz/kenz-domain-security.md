---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kenzwoman.com
  spf: true
hosts:
- cert_expires: Sep 15 02:32:58 2026 GMT
  host: kenzwoman.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kenz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kenz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kenz
provider_slug: kenz
slug: kenz-domain-security
source_filename: kenz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kenzwoman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:32:58 2026 GMT\n  hsts: null\ndomains:\n- domain: kenzwoman.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kenz/refs/heads/main/security/kenz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
