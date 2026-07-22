---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: neuron23.com
  spf: true
hosts:
- cert_expires: Sep 28 12:53:15 2026 GMT
  host: neuron23.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuron23 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neuron23, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neuron23
provider_slug: neuron23
slug: neuron23-domain-security
source_filename: neuron23-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neuron23.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neuron23.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuron23/refs/heads/main/security/neuron23-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health Tech
- Biotechnology
- Precision Medicine
- Neuroscience
- Pharmaceuticals
- Drug Discovery
- Parkinsons Disease
---
