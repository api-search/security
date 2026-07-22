---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: latentlabs.com
  spf: true
hosts:
- cert_expires: Aug 27 14:26:49 2026 GMT
  host: www.latentlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Latent Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latent Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Latent Labs
provider_slug: latent-labs
slug: latent-labs-domain-security
source_filename: latent-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.latentlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 14:26:49 2026 GMT\n  hsts: false\ndomains:\n- domain: latentlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latent-labs/refs/heads/main/security/latent-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Generative AI
- Foundation Models
- Biology
- Programmable Biology
- Protein Design
- Drug Discovery
- Drug Design
- Antibodies
- Macrocycles
- Protein Binders
- Biotech
- Pharmaceutical
- Life Sciences
- AlphaFold
- Computational Biology
---
