---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: benefitfocus.com
  spf: true
hosts:
- cert_expires: Jan  3 07:59:26 2027 GMT
  host: www.benefitfocus.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benefitfocus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Benefitfocus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Benefitfocus
provider_slug: benefitfocus
slug: benefitfocus-domain-security
source_filename: benefitfocus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benefitfocus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 07:59:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: benefitfocus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/benefitfocus/security/benefitfocus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Benefits
- Human Resources
- Software-as-a-Service
- Healthcare
- Cloud
---
