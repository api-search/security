---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Dec 18 16:17:45 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Augmented Intelligence Aui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmented Intelligence (AUI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Augmented Intelligence (AUI)
provider_slug: augmented-intelligence-aui
slug: augmented-intelligence-aui-domain-security
source_filename: augmented-intelligence-aui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:17:45 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmented-intelligence-aui/refs/heads/main/security/augmented-intelligence-aui-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
