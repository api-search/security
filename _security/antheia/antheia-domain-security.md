---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antheia.bio
  spf: true
hosts:
- cert_expires: Sep 13 02:30:25 2026 GMT
  host: antheia.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antheia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antheia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antheia
provider_slug: antheia
slug: antheia-domain-security
source_filename: antheia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antheia.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:30:25 2026 GMT\n  hsts: false\ndomains:\n- domain: antheia.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antheia/refs/heads/main/security/antheia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Synthetic Biology
- Pharmaceuticals
- Manufacturing
- Supply Chain
- Fermentation
- Active Pharmaceutical Ingredients
- Drug Shortages
---
