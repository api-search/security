---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clearnotehealth.com
  spf: true
hosts:
- cert_expires: Sep 15 22:48:34 2026 GMT
  host: www.clearnotehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluestar Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearNote Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ClearNote Health
provider_slug: bluestar-genomics
slug: bluestar-genomics-domain-security
source_filename: bluestar-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearnotehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:48:34 2026 GMT\n  hsts: false\ndomains:\n- domain: clearnotehealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluestar-genomics/refs/heads/main/security/bluestar-genomics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health
- Biotechnology
- Genomics
- Epigenomics
- Cancer Detection
- Diagnostics
- Liquid Biopsy
- Precision Medicine
- Life Sciences
---
