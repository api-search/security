---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buerklin.com
  spf: true
hosts:
- cert_expires: Dec 24 20:40:12 2026 GMT
  host: www.buerklin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buerklin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buerklin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buerklin
provider_slug: buerklin
slug: buerklin-domain-security
source_filename: buerklin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buerklin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:40:12 2026 GMT\n  hsts: false\ndomains:\n- domain: buerklin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/buerklin/security/buerklin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
