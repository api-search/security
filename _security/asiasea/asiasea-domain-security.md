---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asiasea.com
  spf: true
hosts:
- host: www.asiasea.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asiasea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asiasea, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Asiasea
provider_slug: asiasea
slug: asiasea-domain-security
source_filename: asiasea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asiasea.com\n  https: false\ndomains:\n- domain: asiasea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asiasea/refs/heads/main/security/asiasea-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Seafood
- Catering
- China
- Supplier
---
