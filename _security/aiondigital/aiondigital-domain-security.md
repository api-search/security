---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aiondigital.com
  spf: true
hosts:
- cert_expires: Mar 18 11:28:53 2027 GMT
  host: aiondigital.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiondigital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aion Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aion Digital
provider_slug: aiondigital
slug: aiondigital-domain-security
source_filename: aiondigital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiondigital.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 11:28:53 2027 GMT\n  hsts: false\ndomains:\n- domain: aiondigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiondigital/refs/heads/main/security/aiondigital-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Banking
- Financial Services
- Digital Banking
- Fintech
- Open Banking
- eKYC
- Identity Verification
- Onboarding
- Artificial Intelligence
- Bahrain
- Middle East
---
