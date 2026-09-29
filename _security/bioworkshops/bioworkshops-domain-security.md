---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioworkshops.com
  spf: true
hosts:
- cert_expires: Jan 31 06:28:27 2027 GMT
  host: www.bioworkshops.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioworkshops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bioworkshops, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bioworkshops
provider_slug: bioworkshops
slug: bioworkshops-domain-security
source_filename: bioworkshops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioworkshops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 06:28:27 2027 GMT\n  hsts: false\ndomains:\n- domain: bioworkshops.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioworkshops/refs/heads/main/security/bioworkshops-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biologics
- CDMO
- AntibodyTherapeutics
- Biosimilars
---
