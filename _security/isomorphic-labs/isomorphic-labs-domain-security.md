---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: isomorphiclabs.com
  spf: true
hosts:
- cert_expires: Sep 16 06:47:12 2026 GMT
  host: www.isomorphiclabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Isomorphic Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Isomorphic Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Isomorphic Labs
provider_slug: isomorphic-labs
slug: isomorphic-labs-domain-security
source_filename: isomorphic-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.isomorphiclabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:47:12 2026 GMT\n  hsts: false\ndomains:\n- domain: isomorphiclabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isomorphic-labs/refs/heads/main/security/isomorphic-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Drug Discovery
- Pharmaceutical
- Life Sciences
- Biotechnology
- Computational Biology
- Protein Structure
- AlphaFold
- Generative AI
- Foundation Models
- Small Molecules
- Biologics
- Oncology
- Immunology
- Alphabet
- DeepMind
---
