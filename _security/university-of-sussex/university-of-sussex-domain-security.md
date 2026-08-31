---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sussex.ac.uk
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.sussex.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: idp.sussex.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: okta.sussex.ac.uk
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Sussex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Sussex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Sussex
provider_slug: university-of-sussex
slug: university-of-sussex-domain-security
source_filename: university-of-sussex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sussex.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: idp.sussex.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\n- host: okta.sussex.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: sussex.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/security/university-of-sussex-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Public Research University
- Identity Federation
- Research Repository
- Library
- Learning Management
- Research
- Open Access
---
