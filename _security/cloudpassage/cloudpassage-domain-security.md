---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fidelissecurity.com
  spf: true
hosts:
- cert_expires: Dec 14 20:01:39 2026 GMT
  host: fidelissecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudpassage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudPassage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CloudPassage
provider_slug: cloudpassage
slug: cloudpassage-domain-security
source_filename: cloudpassage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fidelissecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 20:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fidelissecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudpassage/refs/heads/main/security/cloudpassage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
