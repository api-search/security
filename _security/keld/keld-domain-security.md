---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keld.co
  spf: true
hosts:
- cert_expires: Dec  3 19:45:18 2026 GMT
  host: keld.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keld, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keld
provider_slug: keld
slug: keld-domain-security
source_filename: keld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keld.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 19:45:18 2026 GMT\n  hsts: false\ndomains:\n- domain: keld.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/keld/security/keld-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI inference
- Marketplace
- Model marketplace
- Enterprise AI
---
