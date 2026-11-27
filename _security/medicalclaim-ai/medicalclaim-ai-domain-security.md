---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medicalclaim.ai
  spf: true
hosts:
- cert_expires: Feb 11 04:23:25 2027 GMT
  host: medicalclaim.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MedicalClaim.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedicalClaim.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MedicalClaim.ai
provider_slug: medicalclaim-ai
slug: medicalclaim-ai-domain-security
source_filename: medicalclaim-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medicalclaim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 04:23:25 2027 GMT\n  hsts: false\ndomains:\n- domain: medicalclaim.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/medicalclaim-ai/security/medicalclaim-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Billing
- Artificial Intelligence
- Claims
---
