---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axiommath.ai
  spf: true
hosts:
- cert_expires: Dec  4 05:09:22 2026 GMT
  host: axiommath.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axiommath Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axiom
provider_slug: axiommath-ai
slug: axiommath-ai-domain-security
source_filename: axiommath-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiommath.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 05:09:22 2026 GMT\n  hsts: false\ndomains:\n- domain: axiommath.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/axiommath-ai/security/axiommath-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mathematics
- FormalVerification
- Research
- AI
---
