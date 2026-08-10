---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alamarbio.com
  spf: true
hosts:
- cert_expires: Sep  8 22:26:20 2026 GMT
  host: alamarbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alamar Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alamar Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alamar Biosciences
provider_slug: alamar-biosciences
slug: alamar-biosciences-domain-security
source_filename: alamar-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alamarbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:26:20 2026 GMT\n  hsts: false\ndomains:\n- domain: alamarbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alamar-biosciences/refs/heads/main/security/alamar-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Proteomics
- Life Sciences
- Biotechnology
- Biomarkers
- Diagnostics
- Bioinformatics
- Laboratory Instruments
- Open Source
---
