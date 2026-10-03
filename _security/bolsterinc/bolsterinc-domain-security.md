---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bolster.ai
  spf: true
hosts:
- cert_expires: Nov  4 22:05:40 2026 GMT
  host: bolster.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bolsterinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolsterinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bolsterinc
provider_slug: bolsterinc
slug: bolsterinc-domain-security
source_filename: bolsterinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bolster.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 22:05:40 2026 GMT\n  hsts: null\ndomains:\n- domain: bolster.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolsterinc/refs/heads/main/security/bolsterinc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
