---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lumos-pharma.com
  spf: true
hosts:
- cert_expires: Dec  9 17:45:45 2026 GMT
  host: lumos-pharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumos Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumos Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumos Pharma
provider_slug: lumos-pharma
slug: lumos-pharma-domain-security
source_filename: lumos-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumos-pharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 17:45:45 2026 GMT\n  hsts: false\ndomains:\n- domain: lumos-pharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lumos-pharma/security/lumos-pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharma
- Rare Diseases
- Clinical Trials
- Growth Hormone
---
