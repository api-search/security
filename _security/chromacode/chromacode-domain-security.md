---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chromacode.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: chromacodecloud.com
  spf: false
hosts:
- cert_expires: Nov  2 22:01:56 2026 GMT
  host: www.chromacode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: chromacodecloud.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chromacode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChromaCode, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ChromaCode
provider_slug: chromacode
slug: chromacode-domain-security
source_filename: chromacode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chromacode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 22:01:56 2026 GMT\n  hsts: false\n- host: chromacodecloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chromacode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: chromacodecloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chromacode/refs/heads/main/security/chromacode-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Molecular Diagnostics
- Genomics
- Oncology
- PCR
- Life Sciences
- Healthcare
- Bioinformatics
- Clinical Diagnostics
- Cloud Software
---
