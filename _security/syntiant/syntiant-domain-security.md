---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syntiant.com
  spf: true
hosts:
- cert_expires: Oct 28 17:51:08 2026 GMT
  host: www.syntiant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syntiant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syntiant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Syntiant
provider_slug: syntiant
slug: syntiant-domain-security
source_filename: syntiant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syntiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:51:08 2026 GMT\n  hsts: false\ndomains:\n- domain: syntiant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syntiant/refs/heads/main/security/syntiant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Edge AI
- Artificial Intelligence
- Machine Learning
- TinyML
- Neural Processors
- Embedded Systems
- Sensors
- Microphones
- Consumer Electronics
- Hardware
---
