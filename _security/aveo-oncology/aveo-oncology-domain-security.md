---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aveooncology.com
  spf: true
hosts:
- cert_expires: Dec 22 22:17:36 2026 GMT
  host: www.aveooncology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aveo Oncology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVEO Oncology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AVEO Oncology
provider_slug: aveo-oncology
slug: aveo-oncology-domain-security
source_filename: aveo-oncology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aveooncology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 22:17:36 2026 GMT\n  hsts: false\ndomains:\n- domain: aveooncology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aveo-oncology/security/aveo-oncology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Oncology
- Biopharmaceutical
- Cancer
- Pharmaceuticals
- Partnerships
---
