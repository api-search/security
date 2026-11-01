---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sagimet.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.sagimet.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sagimet Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sagimet Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sagimet Biosciences
provider_slug: sagimet-biosciences
slug: sagimet-biosciences-domain-security
source_filename: sagimet-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sagimet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sagimet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sagimet-biosciences/security/sagimet-biosciences-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fatty Acid Synthase Inhibitors
- Dermatology
- Metabolic Disease
- Oncology
---
