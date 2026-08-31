---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parsebiosciences.com
  spf: true
hosts:
- cert_expires: Sep 26 18:30:43 2026 GMT
  host: www.parsebiosciences.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parse Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parse Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parse Biosciences
provider_slug: parse-biosciences
slug: parse-biosciences-domain-security
source_filename: parse-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parsebiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:30:43 2026 GMT\n  hsts: false\ndomains:\n- domain: parsebiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parse-biosciences/refs/heads/main/security/parse-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Genomics
- Single-Cell Sequencing
- Bioinformatics
- Scientific Software
- Data Analysis
- Laboratory
- Research
---
