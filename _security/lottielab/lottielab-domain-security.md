---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lottielab.com
  spf: true
hosts:
- cert_expires: Sep 13 00:00:51 2026 GMT
  host: www.lottielab.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lottielab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lottielab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lottielab
provider_slug: lottielab
slug: lottielab-domain-security
source_filename: lottielab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lottielab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:00:51 2026 GMT\n  hsts: false\ndomains:\n- domain: lottielab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lottielab/refs/heads/main/security/lottielab-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Animation
- Motion Design
- Lottie
- Design Tools
- Developer Tools
- Web Components
- SDK
- CDN
- Creative
---
