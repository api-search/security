---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mayo.edu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mayoclinic.org
  spf: true
hosts:
- host: apiportal.mcc.mayo.edu
  https: false
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.mayoclinic.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mayo Clinic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mayo Clinic, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mayo Clinic
provider_slug: mayo-clinic
slug: mayo-clinic-domain-security
source_filename: mayo-clinic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiportal.mcc.mayo.edu\n  https: false\n- host: www.mayoclinic.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mayo.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mayoclinic.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mayo-clinic/refs/heads/main/security/mayo-clinic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Clinical Data
- Healthcare
- Hospital
- Medical
---
