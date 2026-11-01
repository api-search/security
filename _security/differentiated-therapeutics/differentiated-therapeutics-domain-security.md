---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dxtherapeutics.com
  spf: true
hosts:
- cert_expires: Jan 10 15:56:03 2027 GMT
  host: www.dxtherapeutics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Differentiated Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Differentiated Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Differentiated Therapeutics
provider_slug: differentiated-therapeutics
slug: differentiated-therapeutics-domain-security
source_filename: differentiated-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dxtherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:56:03 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: dxtherapeutics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/differentiated-therapeutics/security/differentiated-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Therapeutics
- Protein Degradation
- Drug Discovery
- Artificial Intelligence
- Biophysics
- chemoproteomics
- Molecular Simulation
---
