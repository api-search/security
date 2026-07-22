---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fftai.com
  spf: true
hosts:
- cert_expires: Dec  2 09:05:03 2026 GMT
  host: fftai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fourier Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fourier Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fourier Intelligence
provider_slug: fourier-intelligence
slug: fourier-intelligence-domain-security
source_filename: fourier-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fftai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 09:05:03 2026 GMT\n  hsts: false\ndomains:\n- domain: fftai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourier-intelligence/refs/heads/main/security/fourier-intelligence-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health Tech
- Robotics
- Rehabilitation Robotics
- Humanoid Robots
- Exoskeleton
- SDK
---
