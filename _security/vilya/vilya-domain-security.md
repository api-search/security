---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vilya.ai
  spf: true
hosts:
- cert_expires: Sep 21 20:04:16 2026 GMT
  host: vilya.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vilya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vilya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vilya
provider_slug: vilya
slug: vilya-domain-security
source_filename: vilya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vilya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:04:16 2026 GMT\n  hsts: false\ndomains:\n- domain: vilya.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vilya/refs/heads/main/security/vilya-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Artificial Intelligence
- Computational Biology
- Macrocycles
- Therapeutics
- Life Sciences
- Protein Design
---
