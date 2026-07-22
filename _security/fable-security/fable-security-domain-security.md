---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fablesecurity.com
  spf: true
hosts:
- cert_expires: Oct 13 20:22:45 2026 GMT
  host: www.fablesecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fable Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fable Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fable Security
provider_slug: fable-security
slug: fable-security-domain-security
source_filename: fable-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fablesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:22:45 2026 GMT\n  hsts: false\ndomains:\n- domain: fablesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fable-security/refs/heads/main/security/fable-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Human Risk Management
- Security Awareness Training
- Phishing Simulation
- Behavioral Security
- Compliance Training
- Security
---
