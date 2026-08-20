---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kcl.ac.uk
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.kcl.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 11:02:03 2026 GMT
  host: docs.er.kcl.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:22:03 2026 GMT
  host: ai.create.kcl.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kings College London Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for King''s College London, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: King's College London
provider_slug: kings-college-london
slug: kings-college-london-domain-security
source_filename: kings-college-london-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kcl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.er.kcl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:02:03 2026 GMT\n  hsts: false\n- host: ai.create.kcl.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:22:03 2026 GMT\n  hsts: null\ndomains:\n- domain: kcl.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kings-college-london/refs/heads/main/security/kings-college-london-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Russell Group
- United Kingdom
- London
- Research
- Research Computing
- Artificial Intelligence
- Institutional Repository
- Identity Federation
- OAI-PMH
- Library
---
