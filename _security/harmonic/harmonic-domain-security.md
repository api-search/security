---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: harmonic.fun
  spf: true
hosts:
- cert_expires: Jan 31 17:05:33 2027 GMT
  host: www.harmonic.fun
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 20:39:21 2026 GMT
  host: aristotle.harmonic.fun
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harmonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harmonic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Harmonic
provider_slug: harmonic
slug: harmonic-domain-security
source_filename: harmonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harmonic.fun\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 17:05:33 2027 GMT\n  hsts: false\n- host: aristotle.harmonic.fun\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:39:21 2026 GMT\n  hsts: false\ndomains:\n- domain: harmonic.fun\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic/refs/heads/main/security/harmonic-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- Mathematics
- Formal Verification
- Theorem Proving
- Lean
- Machine Reasoning
- Developer Tools
---
