---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dmarc@converge-bio.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: converge-bio.com
  spf: true
hosts:
- cert_expires: Sep 29 02:47:18 2026 GMT
  host: converge-bio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Converge Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Converge Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Converge Bio
provider_slug: converge-bio
slug: converge-bio-domain-security
source_filename: converge-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: converge-bio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: converge-bio.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dmarc@converge-bio.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/converge-bio/refs/heads/main/security/converge-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Drug Discovery
- Generative AI
- Biotech
- Pharmaceutical
- Antibody Design
- Genomics
- Life Sciences
- Machine Learning
---
