---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: twinstrandbio.com
  spf: true
hosts:
- cert_expires: Nov  2 22:23:23 2026 GMT
  host: twinstrandbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Twinstrand Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TwinStrand Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TwinStrand Biosciences
provider_slug: twinstrand-biosciences
slug: twinstrand-biosciences-domain-security
source_filename: twinstrand-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twinstrandbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 22:23:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: twinstrandbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twinstrand-biosciences/refs/heads/main/security/twinstrand-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Biotechnology
- Life Sciences
- DNA Sequencing
- Next-Generation Sequencing
- Oncology
- Genetic Toxicology
- Diagnostics
- Bioinformatics
- Research
- Content
---
