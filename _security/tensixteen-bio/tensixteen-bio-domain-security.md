---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tensixteen.bio
  spf: true
hosts:
- cert_expires: Oct  4 10:54:04 2026 GMT
  host: tensixteen.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensixteen Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TenSixteen Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TenSixteen Bio
provider_slug: tensixteen-bio
slug: tensixteen-bio-domain-security
source_filename: tensixteen-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tensixteen.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:54:04 2026 GMT\n  hsts: false\ndomains:\n- domain: tensixteen.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensixteen-bio/refs/heads/main/security/tensixteen-bio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Life Sciences
- Biotechnology
- Precision Medicine
- Genomics
- Clonal Hematopoiesis
- Therapeutics
- Diagnostics
---
