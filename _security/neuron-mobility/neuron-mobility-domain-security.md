---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rideneuron.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: rideneuron.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuron Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neuron Mobility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Neuron Mobility
provider_slug: neuron-mobility
slug: neuron-mobility-domain-security
source_filename: neuron-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rideneuron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rideneuron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuron-mobility/refs/heads/main/security/neuron-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Micromobility
- E-Scooter
- E-Bike
- Transportation
- Shared Mobility
- IoT
- Smart Cities
---
