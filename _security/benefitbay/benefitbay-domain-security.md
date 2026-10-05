---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: benefitbay.com
  spf: true
hosts:
- cert_expires: Nov 28 15:33:25 2026 GMT
  host: www.benefitbay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Benefitbay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BenefitBay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BenefitBay
provider_slug: benefitbay
slug: benefitbay-domain-security
source_filename: benefitbay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benefitbay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: benefitbay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/benefitbay/refs/heads/main/security/benefitbay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- ICHRA
- Benefits
- Health Tech
- Software-as-a-Service
- Employee Benefits
---
