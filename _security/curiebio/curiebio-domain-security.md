---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curie.bio
  spf: true
hosts:
- cert_expires: Aug 16 19:25:42 2026 GMT
  host: curie.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curiebio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curie.Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curie.Bio
provider_slug: curiebio
slug: curiebio-domain-security
source_filename: curiebio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curie.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:25:42 2026 GMT\n  hsts: false\ndomains:\n- domain: curie.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curiebio/refs/heads/main/security/curiebio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Biotechnology
- Life Sciences
- Drug Discovery
- Therapeutics
- Seed Investment
- Accelerator
---
