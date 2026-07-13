---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cradle.bio
  spf: true
hosts:
- cert_expires: Sep 12 21:30:27 2026 GMT
  host: www.cradle.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 01:55:53 2026 GMT
  host: docs.cradle.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 05:06:10 2026 GMT
  host: app.cradle.bio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cradle Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cradle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cradle
provider_slug: cradle-bio
slug: cradle-bio-domain-security
source_filename: cradle-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cradle.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cradle.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:55:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.cradle.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:06:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cradle.bio\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cradle-bio/refs/heads/main/security/cradle-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Protein Engineering
- Generative Biology
- Generative AI
- Foundation Models
- Machine Learning
- Biotechnology
- Biopharma
- Drug Discovery
- Antibody Discovery
- Enzyme Engineering
- Vaccines
- Therapeutic Peptides
- Industrial Biotech
- Synthetic Biology
- Computational Biology
- Wet Lab
- Life Sciences
- Custom Predictors
---
