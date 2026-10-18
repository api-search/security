---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carihealth.com
  spf: true
hosts:
- cert_expires: Dec 30 03:53:40 2026 GMT
  host: carihealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cari Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cari Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cari Health
provider_slug: cari-health
slug: cari-health-domain-security
source_filename: cari-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 03:53:40 2026 GMT\n  hsts: false\ndomains:\n- domain: carihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cari-health/refs/heads/main/security/cari-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Health Tech
- ClinicalData
- OpioidTreatment
- Personalized Medicine
---
