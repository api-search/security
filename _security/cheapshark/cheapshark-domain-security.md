---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cheapshark.com
  spf: true
hosts:
- cert_expires: Sep 24 19:17:21 2026 GMT
  host: www.cheapshark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cheapshark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CheapShark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CheapShark
provider_slug: cheapshark
slug: cheapshark-domain-security
source_filename: cheapshark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cheapshark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 19:17:21 2026 GMT\n  hsts: false\ndomains:\n- domain: cheapshark.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cheapshark/refs/heads/main/security/cheapshark-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Games And Comics
- Public APIs
---
