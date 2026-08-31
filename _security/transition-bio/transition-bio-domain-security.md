---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transitionbio.com
  spf: true
hosts:
- cert_expires: Oct 19 17:49:43 2026 GMT
  host: transitionbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transition Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transition Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transition Bio
provider_slug: transition-bio
slug: transition-bio-domain-security
source_filename: transition-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transitionbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 17:49:43 2026 GMT\n  hsts: false\ndomains:\n- domain: transitionbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transition-bio/refs/heads/main/security/transition-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Life Sciences
- Machine-Learning
- Artificial Intelligence
- Microfluidics
- Proteomics
- Therapeutics
- Neurodegeneration
---
