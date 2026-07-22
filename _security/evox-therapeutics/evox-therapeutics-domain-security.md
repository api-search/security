---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evoxtherapeutics.com
  spf: true
hosts:
- cert_expires: Aug 28 15:02:54 2026 GMT
  host: www.evoxtherapeutics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evox Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evox Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evox Therapeutics
provider_slug: evox-therapeutics
slug: evox-therapeutics-domain-security
source_filename: evox-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evoxtherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 15:02:54 2026 GMT\n  hsts: false\ndomains:\n- domain: evoxtherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evox-therapeutics/refs/heads/main/security/evox-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Gene Therapy
- Genetic Medicine
- Exosomes
- Neurodegenerative Disease
- CRISPR
---
