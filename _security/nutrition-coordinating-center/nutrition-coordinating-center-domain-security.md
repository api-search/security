---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umn.edu
  spf: true
hosts:
- cert_expires: May 15 19:02:42 2027 GMT
  host: www.ncc.umn.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nutrition Coordinating Center (University of Minnesota) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutrition Coordinating Center (University of Minnesota), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nutrition Coordinating Center (University of Minnesota)
provider_slug: nutrition-coordinating-center
slug: nutrition-coordinating-center-domain-security
source_filename: nutrition-coordinating-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncc.umn.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 15 19:02:42 2027 GMT\n  hsts: false\ndomains:\n- domain: umn.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nutrition-coordinating-center/security/nutrition-coordinating-center-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Nutrition
- Dietary Assessment
- food-composition
- Research
- University
---
