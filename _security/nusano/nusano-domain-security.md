---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nusano.com
  spf: true
hosts:
- cert_expires: Oct 10 00:13:08 2026 GMT
  host: nusano.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nusano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nusano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nusano
provider_slug: nusano
slug: nusano-domain-security
source_filename: nusano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nusano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:13:08 2026 GMT\n  hsts: false\ndomains:\n- domain: nusano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/security/nusano-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Radioisotopes
- Nuclear Medicine
- Life Sciences
- Healthcare
- Oncology
- Radiopharmaceuticals
- Physics
- Advanced Manufacturing
- Nuclear Energy
- HALEU
- Critical Minerals
---
