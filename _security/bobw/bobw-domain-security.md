---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bobw.co
  spf: true
hosts:
- cert_expires: Dec 30 13:55:13 2026 GMT
  host: bobw.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bobw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bobw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bobw
provider_slug: bobw
slug: bobw-domain-security
source_filename: bobw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bobw.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:55:13 2026 GMT\n  hsts: false\ndomains:\n- domain: bobw.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bobw/refs/heads/main/security/bobw-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Accommodation
- Sustainability
- Europe
- Short-Stay
---
