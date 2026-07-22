---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: twig.bio
  spf: true
hosts:
- cert_expires: Sep  5 03:37:54 2026 GMT
  host: twig.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Twig
provider_slug: twig
slug: twig-domain-security
source_filename: twig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twig.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:37:54 2026 GMT\n  hsts: false\ndomains:\n- domain: twig.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twig/refs/heads/main/security/twig-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Bioengineering
- Synthetic Biology
- Artificial Intelligence
- Machine Learning
- Sustainability
- Ingredients
- Fermentation
---
