---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sentibio.com
  spf: true
hosts:
- cert_expires: Sep 18 20:10:52 2026 GMT
  host: www.sentibio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Senti Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Senti Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Senti Biosciences
provider_slug: senti-biosciences
slug: senti-biosciences-domain-security
source_filename: senti-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentibio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:10:52 2026 GMT\n  hsts: false\ndomains:\n- domain: sentibio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/senti-biosciences/refs/heads/main/security/senti-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Biotechnology
- Cell and Gene Therapy
- Gene Circuits
- Oncology
- Therapeutics
- Life Sciences
---
