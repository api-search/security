---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qmul.ac.uk
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.qmul.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:24:49 2026 GMT
  host: qmro.qmul.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Queen Mary University Of London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Queen Mary University of London, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Queen Mary University of London
provider_slug: queen-mary-university-of-london
slug: queen-mary-university-of-london-domain-security
source_filename: queen-mary-university-of-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qmul.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\n- host: qmro.qmul.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:24:49 2026 GMT\n  hsts: false\ndomains:\n- domain: qmul.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queen-mary-university-of-london/refs/heads/main/security/queen-mary-university-of-london-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- OAI-PMH
- Library
- United Kingdom
- London
---
