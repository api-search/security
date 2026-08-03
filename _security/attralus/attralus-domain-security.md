---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: attralus.com
  spf: true
hosts:
- cert_expires: Sep 29 11:13:06 2026 GMT
  host: attralus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Attralus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Attralus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Attralus
provider_slug: attralus
slug: attralus-domain-security
source_filename: attralus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attralus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:13:06 2026 GMT\n  hsts: false\ndomains:\n- domain: attralus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attralus/refs/heads/main/security/attralus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Health
- Clinical Trials
- Therapeutics
- Rare Disease
- Amyloidosis
- Monoclonal Antibodies
- Molecular Imaging
- Neurodegeneration
- Drug Development
---
